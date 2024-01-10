<script setup>
 function doSomething(){
  console.log('doSomething');
 }
</script>

<template>
  <section>
    <h1>Events Vue.js</h1>
    <!-- <form action="https://google.com/search"> -->
      <div class="div">
        <input @click="console.log('World')" type="text" name="q"/>
      <button @click="console.log('hi')" class="bg-red-500">
        Do Something
      </button>
      </div>
    <!-- </form> -->
  </section>
</template>

<style scoped>

</style>
