<template>
  <div class="cards">
      <div class="cards-img">
          <img :src="comicsCover.thumb"  :alt="comicsCover.series" />
      </div>
      <div class="cards-text">
          <p>{{ comicsCover.series }}</p>
      </div>
  </div>
</template>

<script>
export default {
    name: "AppCoverApp",
    
    props: {
        comicsCover: Object
    },
}
</script>

<style lang="scss" scoped>
.cards{
    display: flex;
    flex-wrap: wrap;
    width: calc(100% / 6);
    margin-bottom: 3rem;
    margin-right: 1em;
    color: white;
}

.cards-img{
    width: 100%;
    height: 200px;
    overflow: hidden;
    margin-bottom: 1rem;
}


</style>