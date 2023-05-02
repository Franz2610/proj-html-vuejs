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
@use "../assets/partials/variables" as *;
button:hover{
    background-color: $bg-primary;
    color: white;
    transition: 2s;
    padding: 25px;
}
.btn-success{
    background-color: $btn-green;
}
.features-wrapper{
    background-color: rgb(243, 243, 243);
    margin-top: 100px;
    padding: 100px;
}
.numbers-p {
    font-size: 14px;
    color: $bg-g;
}
span{
    color: $btn-green;
}
button{
    padding-left: 44px;
    padding-right: 44px;
    margin-bottom: 20px;
    margin-top: 50px;
}
.w-30{
    width: 970px;
    margin-left: 200px;
    margin-top: 80px;
}
</style>