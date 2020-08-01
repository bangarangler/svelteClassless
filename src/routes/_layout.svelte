<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
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

<header>
  <h1 class="fake-logo">Fake Logo</h1>
  <Nav {segment} />
</header>

<main class="layout">
  <slot />
</main>

<footer>
  <h3 class="fake-logo">Fake Logo</h3>
  <Nav {segment} />
  <p>&copy; 2020 Jonathan Dain Palacio</p>
</footer>

