<template>
    <div class="text-center">
        <p class="text-uppercase"> enjoy reading on maxcoach</p>
        <h3>Latest on Our Blogs</h3>
        <CardLatest/>
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

</style>