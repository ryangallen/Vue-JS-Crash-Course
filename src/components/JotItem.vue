<template>
  <div class="jot">
    <div>{{jot.time}}</div>
    <p>{{jot.msg}}</p>
  </div>
</template>

<script>
  export default {
    name: "JotItem",
    props: ["jot"]
  }
</script>

<style scoped>
.jot {
  margin-bottom: 32px;
}
.jot>div {
  color: rgba(44, 62, 80, 0.50)
}
</style>
