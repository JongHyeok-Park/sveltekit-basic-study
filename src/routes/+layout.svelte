<script>
  let { children } = $props();
</script>

<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/blog/hello-world">Blog</a>
  <a href="/settings">Settings</a>
  <a href="/add">Add</a>
</nav>

{@render children()}

<style>
  nav {
    background: #eee;
    width: 100%;
    padding: 10px;
  }

  nav > a {
    color: black;
    font-size: 16px;
    text-decoration: none;
  }
</style>