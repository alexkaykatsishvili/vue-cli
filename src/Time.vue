<template>
  <div class="time">
    <h3>What time is it?</h3>
    <h4>Just push a button below!</h4>
    <button type="button" name="button" @click="showCurrentTime">Show</button>
    <p>Your current time is {{time}}</p>
  </div>
</template>

<script>

  export default {
    data () {
      return {
        time: ''
      }
    },
    methods: {
      showCurrentTime () {
        var hms = new Date();
        this.time = hms;
      }
    }
  }
</script>

<style lang="scss">
  .time {
    color: #ccc;
    p {
      color: black;
    }
  }
</style>
