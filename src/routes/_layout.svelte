<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
</script>

<style>
  .fake-logo {
    font-size: var(--baseFontSize);
    margin: 0;
  }
</style>

<header>
  <h1 class="fake-logo">Fake Logo</h1>
  <Nav {segment} />
</header>

<main class="layout">
  <slot />
</main>

