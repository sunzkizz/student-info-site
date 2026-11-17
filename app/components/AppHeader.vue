<!-- AppHeader: website navigation -->
<template>
  <header class="header">
    <div class="header-inner">
      <span class="logo">🎓 CARSU SPACE</span>
      <nav>
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/students">Students</NuxtLink>
        <NuxtLink to="/about">About</NuxtLink>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.header { background: #1ea73c; color: white; }
.header-inner {
  max-width: 960px;
  margin: 0 auto;
  padding: 16px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.logo { font-weight: 700; font-size: 1.2rem; }
nav { display: flex; gap: 16px; }
nav a { color: #dbe4ff; text-decoration: none; }
nav a:hover { color: white; }
/* Nuxt adds this class to the link of the current page */
nav a.router-link-exact-active { color: white; font-weight: 700; border-bottom: 2px solid white; }
</style>
