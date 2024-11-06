<script>
  let menuOpen = false;

  function toggleMenu() {
      menuOpen = !menuOpen;
  }
</script>

<div class="nav-component">
  <div class="nav-logo">
      <!-- Logo here -->
  </div>

  <div class="nav-links" class:active={menuOpen}>
      <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/event">Events</a></li>
          <li><a href="/gallery">Gallery</a></li>
          <li><a href="/contact">Contact</a></li>
          <li class="summa"><a href="https://linktr.ee/magnovite24christkengeri">Register</a></li>
      </ul>
  </div>

  <div class="nav-link-btn">
      <a href="https://linktr.ee/magnovite24christkengeri">Register</a>
  </div>

  <!-- Hamburger icon -->
  <div class="hamburger" on:click={toggleMenu}>
    <span></span>
    <span></span>
    <span></span>
   </div>
</div>