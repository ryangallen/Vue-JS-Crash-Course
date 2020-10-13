<template>
  <Header />
  <Jots v-bind:user="user" />
</template>

<script>
  import 'purecss/build/pure-min.css'
  import 'purecss/build/grids-responsive-min.css'

  import Header from './components/layout/Header'
  import Jots from './components/Jots'

  export default {
    name: 'App',
    components: {
      Header,
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
</style>
