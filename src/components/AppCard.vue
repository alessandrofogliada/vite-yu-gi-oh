<script>
export default{
    name:'AppCard',
    props:{
      info:{
        type: Array,
      }
    }
}
</script>


<template>
  <div class="card">

  </div>

</template>

<style scoped lang="scss">

.card{
    width: calc((100% / 10) - 10px);
    height: 200px;
    background-color: blue;
    color: white;
    border: 4px solid black;
    margin: 5px 5px;
}

.card img{
    width: 100%;
}

h2{
  color: white;
}

</style>