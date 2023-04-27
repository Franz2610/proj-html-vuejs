<template>
    <div class="d-flex ">
        <ul v-for="(nav, index) in navs" :key="index" class="justify-content-center align-items-center gap-1">
            <a class="m-0 text-uppercase d-flex fs-6" href="#">{{ nav.name }} <i class="fa-solid fa-angle-down"></i></a>
        </ul>
    </div>
</template>

<script>
import {navUl} from '../assets/data' ;
    export default {
        name:'TopBar',
        data() {
            return {
                navs: navUl,
            }
        }
    }
</script>

<style lang="scss" scoped>
a{
    text-decoration: none;
    color: white;

    &:hover{
        background-color: white;
        color: blue;
        padding: 10px;
        transition: 2s;
    }
}

</style>