<script>
  export let segment;
</script>

<style>
  [aria-current] {
    position: relative;
    display: inline-block;
  }

  [aria-current]::after {
    position: absolute;
    content: "";
    width: calc(100% - 1em);
    height: 2px;
    background-color: rgb(255, 62, 0);
    display: block;
    bottom: -1px;
  }
</style>

<nav>
  <a aria-current={segment === undefined ? 'page' : undefined} href=".">home</a>
  <a aria-current={segment === 'about' ? 'page' : undefined} href="about">
    about
  </a>

  <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
  <a
    rel="prefetch"
    aria-current={segment === 'blog' ? 'page' : undefined}
    href="blog">
    blog
  </a>
</nav>
