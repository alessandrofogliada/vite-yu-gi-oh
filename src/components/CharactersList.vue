<script>
export default{
    name:'CharactersList'
}

</script>


<template>
    <div class="container">
        <div class="contenitorecard">
            <div class="card">
                <img src="" alt="">
                <span>name</span><br>
                <span>type</span>
            </div>
        </div>
    </div>
</template>


<style scoped lang="scss">

.container{
    background-color:#d48f38 ;
    width: 1000px;
    min-height: 150px;
}

.contenitorecard{
    background-color: white;
    margin: 0 auto;
    width: 800px;
    min-height: 100px;
}

.card{
    width: calc(100% / 5);
    height: 55px;
    margin: 0 10px;
    background-color:blue;
}

</style>