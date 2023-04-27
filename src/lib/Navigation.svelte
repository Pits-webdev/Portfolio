<script>
</script>

<div class="navigation">
  <nav class="container_xl">
    <ul class="menu">
      <li><a href="/" class="link">Logo</a></li>
      <li><a href="/" class="link">Home</a></li>
      <li><a href="/about" class="link">About</a></li>
      <li><a href="/work" class="link">Work</a></li>
    </ul>

    <div class="small_menu">
      <div class="color_theme">Theme</div>
      <div class="contact">
        <a class="link_contact" href="/">Contact</a>
      </div>
    </div>

    <span class="hz_line" />
  </nav>
</div>

<style>
  .navigation {
    width: 100%;
    height: 9vh;
  }

  nav {
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  nav .hz_line {
    position: absolute;
    left: 0;
    bottom: 0;
  }

  .menu,
  .small_menu {
    display: flex;
    align-items: center;
    gap: 7.2rem;
  }

  .link {
    font-size: 1.6rem;
    font-weight: 500;
  }
  .link_contact {
    font-size: 1.8rem;
  }

  .contact a {
    background-color: var(--black);
    color: var(--white);
    padding: 1rem 2rem;
    border-radius: 3rem;
    font-weight: 500;
  }

  .contact a:hover {
    color: var(--primary);
  }
</style>
