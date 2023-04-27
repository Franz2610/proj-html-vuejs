<template>
    <header>
        <div class="d-flex container">
            <img src="/img/light-logo.png" alt="light-logo">
            <TopBar/>
            <div class="searchbar">
                <i class="fa-solid fa-circle-user"></i>
                <input type="text" name="searchBar" id="searchBar" placeholder="Search" class="rounded"/> 
                <i class="fa-solid fa-magnifying-glass"></i>
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
    color: white;
    position: relative;
    height: 750px;
}
.searchbar{
    margin-left: 20px;
}
</style>