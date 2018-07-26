<template>
  <div class="greetings">
    <h1>Hello, {{name}}!</h1>
    <button @click="changeName">Not {{name}}?</button>
  </div>
</template>

<script>

  export default {
    data () {
      return {
        name: 'Alex'
      }
    },
    methods: {
      changeName () {
        this.name = this.name == 'Alex' ? 'Daniel' : 'Alex';
      }
    }
  }

</script>

<style>

</style>
