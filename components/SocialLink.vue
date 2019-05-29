<template lang="pug">
  ul.social__container
    li.item.twitter
      a(href='https://twitter.com/dazi_gomi', target='_blank') Twitter
    li.item.instagram
      a(href='https://www.instagram.com/dazi_gomi/', target='_blank') Instagram
    li.item.steam
      a(href='https://steamcommunity.com/id/dazi_gomi', target='_blank') Steam
    li.item.twitch
      a(href='https://www.twitch.tv/dazi_gomi', target='_blank') Twitch
</template>

<style lang="scss">
  .social__container {
    width: 640px;
    margin: auto;
    display: flex;
    flex-direction: column;
    @include tab {
      width: 50%;
    }

  }

  .item {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    height: auto;
    text-decoration: none;

    + .item {
      margin-top: 10px;
      @include tab {
        margin-top: 4%;
      }
    }

    a {
      position: relative;
      width: auto;
      height: auto;
      padding: 3px 10px;
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
