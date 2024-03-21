<template>
  <header>
    <div class="header">
      <RouterLink to="/" class="nonLink">Vitsekalender</RouterLink>
      <nav class="navbar">
        <RouterLink to="/" class="navLink">Home</RouterLink>
        <RouterLink to="/sporsmal" class="navLink">Home2</RouterLink>
      </nav>
    </div>
  </header>
</template>

<style>
.header {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  background-color: black;
  padding: 20px 40px;
  font-family: monospace;
}
.navbar {
  display: flex;
  flex-direction: row;
  gap: 20px;
}
.navLink {
  color: white;
  font-size: large;
  &:hover {
    font-weight: 900;
  }
}
.nonLink {
  text-decoration: none;
  color: white;
  font-size: x-large;
}
</style>
