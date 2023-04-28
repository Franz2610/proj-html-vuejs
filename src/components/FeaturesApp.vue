<template>
<div class="features-wrapper">
    <div class="text-center container">
        <p class="text-uppercase numbers-p"> choose a course to get started</p>
        <h3 class="mt-3">Latest Featured <span>Courses</span> </h3>
        <div class="w-30">
        <CardFeatures/>
        </div>
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
    margin-top: 100px;
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
    margin-bottom: 100px;
    margin-top: 50px;
}
button:hover{
    background-color: rgba(56, 56, 173, 0.764);
    color: white;
    transition: 2s;
    padding: 25px;
}
.w-30{
    width: 970px;
    margin-left: 200px;
    margin-top: 80px;
}
</style>