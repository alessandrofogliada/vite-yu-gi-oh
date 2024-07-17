<script>
import {store} from "../store"

export default{
    name:"AppSearch",
    props: ['info'],
    data() {
        return {
            store
        }
    },
}
</script>


<template>

<select v-model="store.searchText">
    <option value="0" selected>{{ info.archetype }}</option>
</select>

</template>


<style lang="scss" scoped>

</style>