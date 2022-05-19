<template>
  <section class="pre-footer">
      <div class="container">
          <ul class="prefooter-menu">
              <li v-for="(item, index) in imgIcons" :key="index">
                <img :src="require(`../assets/img/${item.image}`)" alt="">
                <h4> {{ item.text }}</h4>
              </li>
          </ul>
      </div>
  </section>
</template>

<script>

export default {
    name: "AppPreFooter",
    data: function() {
        return {
            imgIcons: [{
                image: "buy-comics-digital-comics.png",
                text: "digital comics",
            },
            {
                image: "buy-comics-merchandise.png",
                text: "dc merchandise",
            },
            {
                image: "buy-comics-subscriptions.png",
                text: "subscription",
            },
            {
                image: "buy-comics-shop-locator.png",
                text: "comic shop locator",
            },
            {
                image: "buy-dc-power-visa.svg",
                text: "dc power visa",
            },
                
            ],
        }
    }
};
</script>

<style lang="scss" scoped>
.pre-footer {
  height: 150px;
  background-color: #0282f9;
  padding: 2rem 0;
  .prefooter-menu {
    display: flex;
    list-style: none;
    text-transform: uppercase;
    color: white;
    li {
      width: calc(100% / 5);
      display: flex;
      align-items: center;
      img {
        width: 25%;
        margin: 0 20px;
      }
      h3 {
        font-size: 8px;
      }
    }
  }
}

</style>