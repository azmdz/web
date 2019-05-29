<template lang="pug">
  section.container
    div
      h1.title.
        dazigomi.com
      ul.link__container
        li
          nuxt-link.link(to="/about") About
        li
          nuxt-link.link(to="/works") Works
        li
          nuxt-link.link(to="/products") Products
        li
          a.link(href="http://blog.dazigomi.com") Blog
</template>

<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    }
  }
</script>

<style>
  .container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-family: Roboto, 'Helvetica Neue', Arial, sans-serif;
  }

  .title {
    display: block;
    font-size: 48px;
    font-weight: 300;
    color: #000;
  }

  .link__container {
    margin: 2.5rem auto;
  }
  .link {
    margin: 0 1rem;
    font-size: 24px;
    text-decoration: none;
    font-weight: 300;
  }

</style>
