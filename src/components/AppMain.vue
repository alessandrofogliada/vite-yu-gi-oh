<script>
import { store } from '../store';

import AppCard from './AppCard.vue';

export default {
    name:'AppMain',
    components:{
        AppCard
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

        <div v-for="item in store.yuGiOhCard" class="cardbinder">
            <AppCard :info="item" />
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