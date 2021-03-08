<template>
  <body>
    <div>
      <webapp-header></webapp-header>
      <webapp-open></webapp-open>
      <webapp-about></webapp-about>
    </div>
    
    
  </body>
</template>

<script>
import header from './views/header.vue'
import open from './views/open.vue'
import about from './views/about.vue'

export default {
  name: 'App',
  components: {
    'webapp-header':header,
    'webapp-open':open,
    'webapp-about':about,
  },
  data: () => ({
     contactTitle: 'Hefur þú fleiri spurningar',
  }),
};

</script>

<style lang="scss">
  body {
    background: linear-gradient(#0bafad, #055756);
    height: 1000px;
  }
  a {
    text-decoration: none;
  }
  h1, h2, h3, h4, h5, p {
    color: white;
    font-family: 'Poppins', sans-serif;
  }
</style>
