<template lang="pug">
  section.container
    h1.title.
      About
    .profile
      h2.subtitle.
        dazi_gomi
    h3.head.
      Skill
    ul.col__list
      li(v-for="item in skills") {{item}}
    h3.head.
      Like
    ul.col__list
      li(v-for="item in likes") {{item}}

    SocialLink

</template>

<script>
  import SocialLink from '~/components/SocialLink.vue'

  export default {
    components: {
      SocialLink
    },
    data() {
      return {
        skills: ["HTML", "CSS", "JavaScript", "MAX/MSP", "AWS", "UI/UX"],
        likes: ["Whisky", "Beer", "Web Design", "Deb Development", "Investment", "Blockchain"]
      }
    },
    head() {
      return {
        title: 'About'
      }
    }
  }
</script>

<style lang="scss" scoped>
  .col__list {
    display: flex;
    flex-wrap: wrap;
    margin: 0 auto;

    > li {
      margin: 0.5rem;
      font-size: 1.6rem;
    }
  }
</style>
