<template>
  <div> 
    <input type="text" @input="onInput" placeholder="search for a video on youtube">
  </div>
</template>

<script>
  export default {
    name: 'SearchBar',
    methods: {
      onInput(event) {
        this.$emit('termChange', event.target.value);
      }
    }
  }
</script>

<style scoped>
input {
  width: 75%;
  padding: 5px;
}

input[placeholder] {
  margin-left: 20px;
}

div {
  text-align: center;
  margin: 20px;
}
</style>

