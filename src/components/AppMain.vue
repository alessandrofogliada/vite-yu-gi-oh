<script>
import { info } from 'sass';
import { store } from '../store';

import AppCard from './AppCard.vue';
import AppSearch from './AppSearch.vue';

export default {
    name:'AppMain',
    components:{
        AppCard,
        AppSearch
    },
    data(){
        return{
            store,
        }
    }
}
</script>


<template>
    <div class="container">

        <div>
            <AppSearch v-for="card in store.yuGiOhCard" :key="card.id" :info="card"/>
        </div>

        <div  class="cardbinder">
            <AppCard v-for="card in store.yuGiOhCard" :key="card.id" :info="card" />
        </div>
 
    </div>
</template>


<style scoped lang="scss">
.container{
    width: 1500px;
    min-height: 1000px;
    background-color: #d48f38;
}

.cardbinder{
    width:1400px;
    min-height: 800px;
    margin: 0 auto;
    background-color: white;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

</style>