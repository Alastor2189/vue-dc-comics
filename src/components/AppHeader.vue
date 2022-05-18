<template>
<div class="container">
  <header class="header">
      <div class="header__logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="header__nav">
          <nav>
              <ul class="header__menu">
                  <li v-for="(item, index) in links" :key="index"><a href="">{{ item.text}}</a></li>
                  
              </ul>
          </nav>
      </div>

  </header>
  </div>
</template>

<script>
export default {
    name: "AppHeader",
    data: function() {
        return {
            links: [
                {
                    url: "#",
                    text: "characters",
                    active: false,
                },
                {
                    url: "#",
                    text: "comics",
                    active: false,
                },
                {
                    url: "#",
                    text: "movies",
                    active: false,
                },
                {
                    url: "#",
                    text: "tv",
                    active: false,
                },
                {
                    url: "#",
                    text: "games",
                    active: false,
                },
                {
                    url: "#",
                    text: "collectibles",
                    active: false,
                },
                {
                    url: "#",
                    text: "videos",
                    active: false,
                },
                {
                    url: "#",
                    text: "characters",
                    active: false,
                },
                {
                    url: "#",
                    text: "fans",
                    active: false,
                },
                {
                    url: "#",
                    text: "news",
                    active: false,
                },
                {
                    url: "#",
                    text: "shop",
                    active: false,
                },
            ]
        }
    },
    components: {
        
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variable.scss";

.header{
    &__logo {
        width: 40%;
    }

    &__nav{
        width: 60%;
    }
    &__menu {
        display: flex;
        justify-content: space-between;
        
        li {
            list-style: none;
            margin-right: 8px;
        }
        a {
            text-decoration: none;
            text-transform: uppercase;
        }
    }
}
</style>


