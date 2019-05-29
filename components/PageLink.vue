<template lang="pug">
  ul.page__container
    li
      nuxt-link.link(to="/about") About
    li
      nuxt-link.link(to="/works") Works
    li
      nuxt-link.link(to="/products") Products
    li
      a.link(href="http://blog.dazigomi.com") Blog
</template>

<style lang="scss">
  .page__container{
    margin: 2rem auto;
    display: flex;
  }
  .link{
    position: relative;
    color: #000;

    &:after,&:before{
      content: '';
      position: absolute;
      width: 100%;
      height: 1px;
      right: 0;
      bottom: 0;
      transition: all 0.18s ease-in;
    }
    &:before{
      background-color: #f00;
    }
    &:after{
      background-color: #000;
    }
    &:hover{
      &:after{
        width: 0;

      }
    }
  }
</style>
