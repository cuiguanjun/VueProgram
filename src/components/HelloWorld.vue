<script setup lang="ts">
import * as cheerio from 'cheerio';
import { BorderBox1 } from '@dataview/datav-vue3';

defineProps<{
  msg: string
}>()

const testCheerio = function(params: any) {
  const $ = cheerio.load("<div><span>Hello World</span></div>");
  let ttt = 30;
}

</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      You’ve successfully created a project with
      <a href="https://vitejs.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>. What's next?
    </h3>
  </div>
  <BorderBox1>
    <!-- <button @click="testCheerio">测试Cheerio</button> -->
    BorderBox1
  
  </BorderBox1>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
