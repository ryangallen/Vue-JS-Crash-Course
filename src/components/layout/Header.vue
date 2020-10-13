<template>
  <header>
    <h1>Jot</h1>
    <div>Write Something Down</div>
  </header>
</template>

<script>
  export default {
    name: "Header"
  }
</script>

<style scoped>
  header {
    border-bottom: 5px solid #a0b8d1;
  }

  header>h1 {
    text-transform: uppercase;
  }

  header>div {
    color: rgba(44, 62, 80, 0.50);
    margin-bottom: 1px;
  }
</style>
