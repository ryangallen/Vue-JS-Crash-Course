<template>
  <header>
    <h1>Jot</h1>
    <div>Write Something Down</div>
  </header>
  <Jots v-bind:user="user" />
</template>

<script>
import Jots from './components/Jots'

export default {
  name: 'App',
  components: {
    Jots
  },
  data() {
    return {
      user: {
        name: "Ryan"
      }
    }
  }
}
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  line-height: 1.45;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

header {
  border-bottom: 5px solid #a0b8d1;
}
header>h1{
  text-transform: uppercase;
}
header>div{
  color: rgba(44, 62, 80, 0.50)
}
</style>
