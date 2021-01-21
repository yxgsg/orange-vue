<template>
  <div id="counter">
    Counter: {{ counter }}
  </div>
  <div id="bind-attribute">
    <span v-bind:title="message">
      Hover your mouse over me for a few secounds to see my dynamically bound title!
    </span>
  </div>
</template>

<script>
export default {
  name: "counter",
  data() {
    return {
      counter: 1,
      message: "You loaded this page on " + new Date().toLocaleString()
    };
  },
  mounted() {
    setInterval(() => {
      this.counter++;
    }, 1900);
  }
};
</script>

<style scoped>

</style>