<script setup>
let {press}=usePress();

const removeWasclicked =(news) =>{
  usePress.removeFromPress(news.id);
}
</script>

<template>
  <div>
    <div class="news">
      <h1>Article</h1>
      <div v-for="news of press" :class="news.type" :key="news.id"><nuxt-link>
        <h3>{{ news.name }}</h3>
          {{news.text.substring(0,97)+"..."}}
          <div class="remove" @click="removeWasclicked(news)">Remove</div>
      </nuxt-link></div>
    </div>
  </div>
</template>

<style scoped></style>
