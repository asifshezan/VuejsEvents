<script setup>
import whatsapp from './components/whatsapp.vue';
import stopevent from './components/stopevent.vue';
import lightbox from './components/lightbox.vue';
import faq from './components/faq.vue';

 function doSomething(){
  console.log('doSomething');
 }

 function detectKeyPress(e){
  console.log('You clicked '+""+ e.key);
 }

 function worksOnlyTabEnter(){
  console.log('you pressed enter');
 }

 function worksOnlyTabSpace(){
  console.log('you pressed Space');
 }

 function submitForm(){
  console.log('you submit the form.');
 }


 
</script>

<template>


<faq/>
<lightbox/>
<stopevent/>
<whatsapp/>



  <section>
    <h1>Events Vue.js</h1>
    <form @submit.prevent="submitForm()" action="https://google.com/search">
      <div class="div">
        <!-- <input @keypress.space="worksOnlyTabSpace()" @keypress.enter="worksOnlyTabEnter()" type="text" name="q" /> -->
        <input type="text" name="q" />
        <!-- <input @keypress="detectKeyPress($event)" type="text" name="q"/> -->
      <!-- <button @click="doSomething()" class="bg-red-500"> -->
        <button type="submit" class="bg-red-500">
        Submit form
      </button>
      </div>
    </form>
  </section>
</template>

<style scoped>

</style>
