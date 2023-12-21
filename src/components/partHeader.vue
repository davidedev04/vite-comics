<script>

export default {
  name: "partHeader",

  data() {

    return {

      links: [
        {
          text: "CHARACTERS",
          url: "#",
          active: false
        },
        {
          text: "COMICS",
          url: "#",
          active: true
        },
        {
          text: "MOVIES",
          url: "#",
          active: false
        },
        {
          text: "TV",
          url: "#",
          active: false
        },
        {
          text: "GAMES",
          url: "#",
          active: false
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          active: false
        },
        {
          text: "VIDEOS",
          url: "#",
          active: false
        },
        {
          text: "FANS",
          url: "#",
          active: false
        },
        {
          text: "NEWS",
          url: "#",
          active: false
        },
        {
          text: "SHOP",
          url: "#",
          active: false
        },
      ]

    }

  }
}

</script>

<template>
  <header>
    <div class="containerHeader">
      <div class="logo">
        <img src="../assets/images/dc-logo.png" alt="logo">
      </div>
      <div class="menu">
        <div class="sections" v-for="object in links">
          <a class="voci" href="object.url" :class="object.active ? 'active' : ''">{{ object.text }}</a>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;

header {
  width: 100vw;
  height: 100px;
  @include displayFlex;
  justify-content: center;
}

.containerHeader {
  @include widthContent;
  @include displayFlex;
  justify-content: space-between;



  img {
    width: 85px;
  }

  .menu {
    display: flex;
    height: 100%;

    .sections {
      height: 100%;
      margin-left: 20px;

      .voci{
        height: 100%;
        text-decoration: none;
        color: #46464e;
        border-bottom: 4px solid #fff;
        font-weight: bold;
        @include displayFlex;
      }

    }

    .voci:hover{
      border-bottom: 4px solid #007ef8;
      color: #007ef8;
    }

    .active {
      border-bottom: 4px solid #007ef8 !important;
      color: #007ef8 !important;
    }

  }
}
</style>