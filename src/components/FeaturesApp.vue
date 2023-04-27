<template>
<div class="features-wrapper mt-5">
    <div class="text-center container">
        <p class="text-uppercase numbers-p "> choose a course to get started</p>
        <h3>Latest Featured <span>Courses</span> </h3>
        <CardFeatures/>
        <button class="btn btn-success"> View all courses <i class="fa-solid fa-arrow-right-long"></i></button>
    </div>
</div>

</template>

<script>
import CardFeatures from './CardFeatures.vue';
    export default {
        name:'FeaturesApp',
        components :{
            CardFeatures
        }
    }
</script>

<style lang="scss" scoped>
.features-wrapper{
    background-color: rgb(243, 243, 243);
}
.numbers-p {
    font-size: 14px;
    color: rgba(172, 167, 167, 0.853);
}
span{
    color: rgb(71, 176, 132);
}
button{
    padding-left: 44px;
    padding-right: 44px;

}

</style>