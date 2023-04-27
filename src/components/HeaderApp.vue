<template>
    <header class="">
        <div class="d-flex container">
            <img src="/img/light-logo.png" alt="light-logo">
            <TopBar/>
            <div class="searchbar">
                <i class="fa-solid fa-cart-shopping"><span>0</span></i>
                <i class="fa-solid fa-circle-user"></i>
                <input type="text" name="searchBar" id="searchBar" placeholder="Search" class="rounded"/> 
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
            <div class="lateralBar text-center">
                <i class="fa-solid fa-cart-arrow-down fs-6 d-block m-2 "></i>
                <i class="fa-solid fa-book fs-6 d-block m-2"></i>
                <i class="fa-solid fa-life-ring fs-6 d-block m-2"></i>
                <i class="fa-solid fa-play fs-6 d-block m-2"></i>
            </div>
        </div>
        <HeaderAppDown/>
    </header>
</template>

<script>
import TopBar from './TopBar.vue';
import HeaderAppDown from './HeaderAppDown.vue'
    export default {
        name:'HeaderApp',
        components :{
            TopBar,
            HeaderAppDown,
        }
    }
</script>

<style lang="scss" scoped>
header{
    background-image: url('/public/img/background-pattern-grid-line.png');
    background-image: url('/public/img/jumbotron-background-wave-small.svg');
    background-image: url('/public/img/jumbotron-background-wave-medium.svg');
    background-image: url('/public/img/jumbotron-background-wave-big.svg');
    background-color: rgb(6, 6, 97);
    position: relative;
    height: 750px;
}
.searchbar{
    margin-left: 20px;
}
i span{
    position: absolute;
    background-color: white;
    color: blue;
    border-radius: 50% ;
    font-size: 8px;
    margin-top: 10px;
    padding: 2px;
}
.fa-cart-shopping{
    position: relative;
    margin-right: 8px;
}
.lateralBar{
position:fixed !important;
position:absolute;
top:100px;
right:0;
margin:0;
padding:0;
width: 30px;
height: 100px;
background-color: white;
}
.searchbar i{
    color: white;
}

</style>