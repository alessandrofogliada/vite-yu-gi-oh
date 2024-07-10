<script>
import AppCard from './AppCard.vue';


export default {
    name:'AppMain',
    components:[
        AppCard
    ]
}
</script>


<template>
    <div class="container">

        <div class="cardbinder">

            <div class="card">
              <AppCard />
            </div>

        </div>

    </div>
</template>


<style>
.container{
    width: 1000px;
    min-height: 1000px;
    background-color: #d48f38;
}

.cardbinder{
    width:900px;
    min-height: 800px;
    margin: 0 auto;
    background-color: white;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.card{
    width: calc(100% / 10);
    height: 160px;
    background-color: blue;
    color: white;
    border: 4px solid black;
    margin: 5px 5px;
}

.card img{
    width: 100%;
}
</style>