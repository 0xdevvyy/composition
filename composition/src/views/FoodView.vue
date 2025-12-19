<script setup>

import { useStorage } from '@/composables/useStorage';

let food = useStorage('food');
let age = useStorage('age');
</script>

<template>
   <div class="food">
        <h1>Food Page</h1>
        <main>
            <p>What is your favourite food: <input type="text" v-model="food"></p>
             <p>What is your age: <input type="text" v-model="age"></p>
        </main>
   </div>
</template>