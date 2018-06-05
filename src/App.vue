<template>
  <div id="app">
    <h1>Word Translator</h1>
    <h5>Powered By Vue.js</h5>
    <TranslateForm></TranslateForm>
  </div>
</template>

<script>
import TranslateForm from './components/TranslateForm'
import TranslateOutput from './components/TranslateOutput'

export default {
  name: 'App',
  components: {
    TranslateForm, TranslateOutput
  }
}
</script>

<style>
body {
  background:#fefefe;
}
</style>
