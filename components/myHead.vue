<script setup></script>

<template>
  <header>

    
    
    <span id="home">
      <nuxt-link to="/"><img src="../imgs/home.svg" alt="home" ></nuxt-link>
    </span>
    
    
    <span id="other">
      <nuxt-link to="/articles/"><img src="../imgs/articles.svg" alt="article"></nuxt-link>
      <nuxt-link to="/contact"><img src="../imgs/contact.svg" alt="contact"></nuxt-link>
    </span>
  </header>
      
</template>

<style scoped>
img{
  width: 3rem;
  height: 3rem;
  margin-right:1rem;
}
#home {
  margin-left:1rem;
}
header{
  margin-top:1rem;
  height: auto;
  width: max-width; 
  justify-items: right;
}
#other{
  float: right;
}
</style>
