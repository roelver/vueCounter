<template>
  <div style="text-align:center">
    <h1>
      Vuejs Counter: {{counter}}
    </h1>
    <button @click="modifyCounter(1)">+</button>
    <button @click="modifyCounter(-1)">-</button>
  </div>
</template>

<script>
    export default {
        data() {
            return {
                counter: 0,
            };
        },
        methods: {
            modifyCounter(val) {
                this.counter += val;
            }
        }
    }
</script>

<style>
</style>
