<template>
  <main>
    <h1>v-model</h1>
    <label>First name:</label>
    <input v-model="name" placeholder="Your name"/>
    <div class="text">
      <h2>{{ name }}</h2>
    </div>
  </main>
</template>

<script lang="ts">
import Input from "./components/Input.vue";
export default {
  name: "App",

  comments: {
    Input,
  },

  data() {
    return {
      name: "",
    };
  },

  methods: {},
};
</script>

<style lang="scss">
main {
  margin: 0 auto;
  text-align: center;
  font: 100 14px arial;
  h1 {
    font: bold 32px arial;
    text-align: center;
    margin: 68px 0;
  }
  label {
    font: bold 16px arial;
    margin-right: 8px;
  }
  input {
    width: 233px;
    padding: 6px 8px;
    border-radius: 4px;
    border: none;
  }
  div.text {
    width: 400px;
    height: 150px;
    background-color: #2b2b2b;
    color: white;
    margin: 16px auto;
    border-radius: 8px;
    padding: 64px 0;
  }
}
</style>
