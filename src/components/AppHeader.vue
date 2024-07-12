<script>
export default { 
    name:'AppHeader',
 }
</script>

 
<template>
    <div class="intestazione">
        <img src="/public/img/Yu-Gi-Oh!.svg" alt="Yu gi oh logo" >
        <h4>Yu-Gi-OH Api</h4>
    </div>
</template>


<style scoped lang="scss">
.intestazione{
    width: 1500px;
    height: 120px;
    background-color: white;
    display: flex;
    align-items: center;
}

.intestazione img{
    width: 150px;
}

h4{
    color: black;
    font-size: 30px;
    text-align: left;
    padding-top: 10px;
}
</style>