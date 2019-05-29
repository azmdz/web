<template lang="pug">
  section.container
    div
      h1.title.
        dazigomi.com
      PageLink
      //- SocialLink
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import SocialLink from '~/components/SocialLink.vue'
  import PageLink from '~/components/PageLink.vue'

  export default {
    components: {
      Logo,
      PageLink,
      SocialLink
    }
  }
</script>

<style>


  .title {
    display: block;
    font-size: 48px;
    font-weight: 300;
    color: #000;
  }

</style>
