<template>
  <header class="main-header">
    <div class="left-menu">
      <h2 class="header-button">TYPING</h2>
    </div>
    <div class="right-menu">
      <p class="header-button">cabinet</p>
    </div>
  </header>
</template>

<style lang="scss">
.main-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  min-height: 10vh;

  .header-button {
    cursor: pointer;
    border-bottom: 1px solid #121212;
    transition: 0.2s ease-in;
  }
  .header-button:hover {
    border-bottom: 1px solid #ffffff;
  }
}
</style>
