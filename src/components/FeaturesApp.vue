<template>
    <div class="text-center features-wrapper">
        <p class="text-uppercase"> choose a course to get started</p>
        <h3>Latest Featured Courses</h3>
        <CardFeatures/>
        <button class="btn btn-success"> View all courses <i class="fa-solid fa-arrow-right-long"></i></button>

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

</style>