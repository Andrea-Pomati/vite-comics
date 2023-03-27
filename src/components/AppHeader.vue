<script>
export default {
    name: "AppHeader",
  data() {
    return {
      
    }
  }
} 

</script>


<template>

<header>

    <div class="container flex-nav">
        
        <img src="/img/dc-logo.png" alt="">

        <ul id="flex-li">
            <li>CHARACHTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
        </ul>



    </div>


</header>



</template>

<style lang="scss" scoped>

header{
    background-color: white;
    color: #6D6D6C;
    font-weight: bold;


}

#flex-li{
    display: flex;
    gap: 10px;
}

.flex-nav{
    display: flex ;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;

}




</style>