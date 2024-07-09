<script>
export default { 
    name:'AppHeader',
    props:[message]
 }
</script>

 
<template>
    <div class="intestazione">
        <h4>{{message}}</h4>
    </div>
</template>


<style scope>
.intestazione{
    width: 1000px;
    height: 120px;
    background-color: white;
}

h4{
    color: black;
    font-size: 30px;
    text-align: left;
    padding-top: 35px;
}
</style>