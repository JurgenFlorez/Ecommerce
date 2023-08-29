<script lang="ts">
export default {
  //options API.A
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increase() {
      this.count += 1; //this.count = this.count +1;
    },
    decrease() {
      this.count -= 1;
    },
  },
  mounted() {
    console.log("El valor iniciar del contador es " + this.count);
  },
};
</script>

<template>
  <h1>Contador: {{ count }}</h1>
  <button @click="increase">Aumentar Contador</button>
  <button @click="decrease">Disminuir Contador</button>
</template>
