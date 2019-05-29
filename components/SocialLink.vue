<template lang="pug">
  section
    h3.head.
      Social Account
    ul.col__list
      li(v-for="item in links" :class="item.color").item
        a(:href="item.url", target="_blank") {{item.name}}
</template>

<script>
  export default {
    data() {
      return {
        links: [
          {
            "name": "Twitter",
            "url": "https://twitter.com/dazi_gomi",
            "color":"twitter"
          },
          {
            "name": "Instagram",
            "url": "https://www.instagram.com/dazi_gomi/",
            "color":"instagram"
          },
          {
            "name": "Steam",
            "url": "https://steamcommunity.com/id/dazi_gomi",
            "color":"steam"
          },
          {
            "name": "Twitch",
            "url": "https://www.twitch.tv/dazi_gomi",
            "color":"twitch"
          }
        ]
      }
    },
    head() {
      return {
        title: 'About'
      }
    }
  }
</script>

<style lang="scss">

  .item {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    height: auto;
    text-decoration: none;
    font-size: 1.4rem;

    + .item {
      margin-top: 1rem;
    }

    a {
      position: relative;
      width: auto;
      height: auto;
      padding: 0.2rem 0.5rem;
      text-decoration: none;
    }

    &.twitter {
      @include hov_link($color_twitter);
    }

    &.twitch {
      @include hov_link($color_twitch);
    }

    &.instagram {
      @include hov_link($color_instagram);
    }

    &.steam {
      @include hov_link($color_steam);
    }
  }
</style>
