<template>
  <div id="app" class="container">
    <h1 class="card-panel purple accent-3 center-align">{{ valor }}</h1>

    <div class="center-align">
      <button v-on:click="contadorSoma()" class="waves-effect waves-light btn">
        +
      </button>
      <button @click="contadorSoma()" class="waves-effect waves-light btn">
        +
      </button>

      <button
        v-on:click="contadorSubtrai()"
        class="waves-effect waves-light red accent-3 btn"
      >
        -
      </button>
      <button
        @click="contadorSubtrai()"
        class="waves-effect waves-light red accent-3 btn"
      >
        -
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      valor: 0,
    };
  },
  methods: {
    contadorSoma() {
      this.valor++;
    },
    contadorSubtrai() {
      this.valor--;
    },
  },
};
</script>

<style>
</style>
