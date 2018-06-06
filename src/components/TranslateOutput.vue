<template>
<h2 class="text-success">{{translatedText}}</h2>
</template>

<script>
  export default {
    name: 'translateOutput',

    props: ['translatedText'],


  }
</script>

<style>
  #transForm{
    border-radius:10px;
    border: 1px #ccc solid;
  }
</style>
