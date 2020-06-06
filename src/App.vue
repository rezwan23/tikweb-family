<template>
  <div>
    <h1>Hello World!</h1>
    <audio controls>
      <source src="/dist/audio/music.mp3" type="audio/mpeg" />
    </audio>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    init() {
      console.log("Hi!! This is GHANI");
    }
  },
  mounted() {
    this.init();
  }
};
</script>

<style scoped>
</style>