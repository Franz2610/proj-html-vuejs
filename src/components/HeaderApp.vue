<template>
    <header>
        <div class="d-flex">
            <h1>Max Coach</h1>
            <TopBar/>
            <i class="fa-solid fa-circle-user"></i>
            <input type="text" name="searchBar" id="searchBar" placeholder="Search" class="rounded-3"/> <i class="fa-solid fa-magnifying-glass"></i>
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

</style>