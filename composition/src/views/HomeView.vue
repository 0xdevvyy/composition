<script setup>
  import { ref } from 'vue';
 import { useFlash } from '@/composables/useFlash';
 import TabableTextArea from '@/components/TabableTextArea.vue';
  let {flash} = useFlash()
  let comment = ref('test value');

  
</script>

<template>
  <main>
   <p>
    <button @click="flash('it works')">click me</button>
   </p>
   <TabableTextArea  style="width: 100%; height: 300px;" v-model="comment"/>
  </main>
</template>
