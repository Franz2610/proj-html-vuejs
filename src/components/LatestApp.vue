<template>
<div class="wrapper-latest">
    <div class="text-center container">
        <p class="text-uppercase number"> enjoy reading on maxcoach</p>
        <h3>Latest on <span>Our Blogs</span> </h3>
        <CardLatest/>
    </div>
</div>
</template>

<script>
import CardLatest from './CardLatest.vue';
    export default {
        name:'FeaturesApp',
        components :{
            CardLatest
        }
    }
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;

.number {
    font-size: 13px;
    color: rgba(172, 167, 167, 0.853);
}
.wrapper-latest{
    background-color: rgb(243, 243, 243);
    padding: 50px;
}
span{
    color: rgb(71, 176, 132);
}

</style>