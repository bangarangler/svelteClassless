<script>
  import Nav from "../components/Nav.svelte";

  export let segment;

  /* const themes = [" ", "dark", "theme", "dark oled"]; */
  const themes = ["", "dark", "theme"];
  /* const icons = ["☀", "🌙", "⚡", "🎱"]; */
  const icons = ["☀", "🌙", "⚡"];
  let index = 0;
  let updatedTheme;
  let removed;
  $: console.log("themes", themes[index]);
  $: console.log("index", index);

  function changeTheme(themes, index) {
    updatedTheme = themes[index];
    removed = themes.filter((th) => th !== updatedTheme);
    switch (document.body.classList) {
      case "":
        document.body.classList.remove("");
        break;
    }
    document.body.classList.add(updatedTheme);
    /* document.body.classList.replace(themes[index - 1], updatedTheme); */
  }
  $: console.log("updatedTheme", updatedTheme);
  $: console.log("removed", removed);
</script>

<style>
  .fake-logo {
    font-size: var(--baseFontSize);
    margin: 0;
  }

  footer .fake-logo {
    margin-bottom: 2%;
  }
</style>

/*
<svelte:body class={themes[index]} />
*/
<header>
  <h1 class="fake-logo">Fake Logo</h1>
  <Nav {segment} />
  <button
    on:click={() => {
      index = (index + 1) % themes.length;
      changeTheme(themes, index);
    }}>
    {icons[index]}
  </button>
</header>

<main class="layout">
  <slot />
</main>

<footer>
  <h3 class="fake-logo">Fake Logo</h3>
  <Nav {segment} />
  <p>&copy; 2020 Jonathan Dain Palacio</p>
</footer>

