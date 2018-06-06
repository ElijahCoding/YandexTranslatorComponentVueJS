<template>
  <div id="translateForm">
    <form @submit="formSubmit">
      <input type="text"
      v-model="textToTranslate"
      placeholder="Enter a Word" />
      <input type="submit" value="Translate">
    </form>
  </div>
</template>

<script>
  export default {
    name: 'translateForm',

    data () {
      return {
        textToTranslate: ''
      }
    },

    methods: {
      formSubmit (e) {
        this.$emit('formSubmit', this.textToTranslate)
        e.preventDefault();
      }
    }
  }
</script>

<style>
  #transForm{
    border-radius:10px;
    border: 1px #ccc solid;
  }
</style>
