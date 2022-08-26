<template>
    <nav>
         <ul>
                <li><a href="">Home</a></li>
                <li><a href="">About me</a></li>
                <li><a href="">Portfolio</a></li>
                <li><a href="">Contact me</a></li>
         </ul>
    </nav>
</template>

<script>
export default{
    name: 'NavBar',
    data(){
        return{

        }
    }
}
</script>


<style>
nav{
    text-align: center;
}
nav ul{
    padding: 0;
     
}
nav li{
    display: inline-block;
    list-style-type: none;
    margin: 2%;
    padding: 15px;
    border: 1px;
    border-radius: 5px;
    border-color: brown;
    background-color:cornflowerblue;
}
nav a{
    color: aliceblue;
}
</style>