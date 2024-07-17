<script>

export default{
    name:'AppCard',
    props: ['info'],
}
</script>


<template>
  <div class="card">
    <img :src="info.card_images[0].image_url" alt="">
    <div class="infocard">
      <h2>{{ info.name }}</h2>
      <h4>{{info.archetype}}</h4>
    </div>
  </div>

</template>

<style scoped lang="scss">

.card{
    width: calc(100% / 8);
    min-height: 200px;
    border: 4px solid black;
    margin: 5px 5px;
}

.infocard{
  background-color: #d48f38;
  color: white;
}

h4{
  color: black;
}

.card img{
    width: 100%;
}

h2{
  color: white;
}

</style>