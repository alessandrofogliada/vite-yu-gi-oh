<script>
import { store } from './store';
import axios from 'axios';

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppSearch from './components/AppSearch.vue';

export default { 
  name: "App",
  components:{
    AppHeader,
    AppMain,
    AppSearch
  },
    data(){
      return{
        store
      }
    },
      methods: {
        getCards() {
          axios.
          get(store.apiUrl)
            .then(res => {
              store.yuGiOhCard = res.data.data
              console.log(res.data.data);
            })
          .catch(err => {
            console.log(err);
          })
        }
      }, 
        created() {
          this.getCards();
        }

}
</script>

<template>
    <AppHeader />
  <main>
    <AppSearch />
    <AppMain />
  </main>
</template>

<style lang="scss">
@use './style/general.scss';


</style>


<!-- <script>

// import di axios 
import axios from 'axios';

import AppHeader from './components/AppHeader.vue'
import AppMainContainer from './components/AppMainContainer.vue'

// import dello state management 
import store from './store';

//  occhio a store 

export default { 
  name: "App",
  components:{
    AppHeader,
    AppMainContainer,
  },
    data() {
      return(
          store
      )
    },
    methods:{
      getCharacters(){
        store.loading = true
        let endPoint = store.apiUrl

        // se si avvia una ricerca da AppSearch aggiunngiamo la query di richiesta 

        if(store.searchText !== ''){
            endPoint += `?${store.apiNamePaeam}=${store.searchText}`
        }

          axios.
          get(endPoint)
          .then(res => {
            store.CardList = res.data.result
            store.loading = false;
            console.log(res.data);
          })
          .catch(err =>{
            store.loading = false;
            console.log(err);
          }
          )
      }
    },
    created() {
      this.getCharacters();
    }
}
</script>

<template>
  <AppHeader message="Yu-Gi-Oh Api"/>
  <main>
    <AppMainContainer />
  </main>

</template>

<style lang="scss">
@use './style/general.scss';
</style> -->
