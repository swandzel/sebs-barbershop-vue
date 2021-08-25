<template>
  <button>{{ buttonText }}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    buttonText: String,
  },
};
</script>

<style scoped>
button {
  color: #e7ecef;
  border: 2px solid #e7ecef;
  font-size: 1.5rem;
  background-color: transparent;
  padding: 10px 20px;
  margin-top: 2rem;
  cursor: pointer;
  text-align: center;
  text-transform: uppercase;
  max-width: 400px;
}
button:hover {
  background-color: #e7ecef;
  color: black;
}
</style>
