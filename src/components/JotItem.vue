<template>
  <div class="jot" v-bind:class="{'done':jot.done}">
    <div>
      {{jot.time}}
      <div class="mark">
        <span @click="$emit('mark-done', jot.id)">
          {{ jot.done ? '&larr;' : '&check;'}}
        </span>
        <span @click="$emit('rem-jot', jot.id)">
          &times;
        </span>
      </div>
    </div>
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
  color: rgba(44, 62, 80, 0.50);
}
.done {
  text-decoration: line-through;
  opacity: 50%;
}
.mark {
  float: right;
  font-weight: 700;
}
.mark>span {
  cursor: pointer;
  padding: 0 5px;
  display: inline-block;
  margin-left: .5em;
}
</style>
