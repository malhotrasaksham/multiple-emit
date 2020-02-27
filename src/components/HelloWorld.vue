<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <button @click="Emit">Emit</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  methods: {
    Emit() {
      this.$emit("emitted", "saksham", 30);
    }
  }
};
</script>
