<template>
  <div id="jot-something">
    <h2>
      Hi {{user.name}}&mdash;have any thoughts to share?
    </h2>
    <form class="pure-form pure-g" @submit="jotItDown">
      <div class="pure-u-1 pure-u-md-21-24">
        <input type="text" name="msg" v-model="msg">
      </div>
      <div class="pure-u-1 pure-u-md-3-24">
        <input type="submit" value="Jot It" class="pure-button">
      </div>
    </form>
  </div>
</template>

<script>
  import { DateTime } from 'luxon';
  import { v4 as uuidv4 } from 'uuid';

  export default {
    name: "JotSomething",
    props: ["user"],
    methods: {
      jotItDown(e) {
        e.preventDefault();

        const newJotItem = {
          id: uuidv4(),
          msg: this.msg,
          time: DateTime.fromISO(new Date().toISOString()).toLocaleString(DateTime.DATETIME_MED),
          done: false
        }
        this.$emit('add-jot', newJotItem);
        this.msg = '';
      }
    },
    data() {
      return {
        msg: ''
      }
    }
  }
</script>

<style scoped>
h2 {
  font-weight: 200;
}
form>div:first-of-type {
  padding: 0 0 .5em 0;
}
@media screen and (min-width: 48em){
  form>div:first-of-type {
    padding: 0 .5em 0 0;
  }
}
form {
  margin-top: .5em;
}
form input {
  width: 100%
}
form input[type="submit"] {
  background-color: rgb(218, 239, 179);
  color: rgb(109, 120, 90);
  border: 1px solid rgba(174, 191, 143, .8);
  height: 100%;
}
#jot-something {
  margin: 2em 0;
}
</style>
