<template>
    <div class="text-center mt-5 mb-5 container">
        <p class="text-uppercase numbers-p"> wanna transform your life?</p>
        <h2 class="mb-5">Glad To <span>Help You</span>  Learn</h2>
        <CardHelp/>
        <div>
            <img src="/public/img/home-6-services-image-1024x411.png" alt="home-service">
        </div>
    </div>
</template>

<script>
import CardHelp from './CardHelp.vue';
    export default {
        name:'HelpApp',
        components :{
            CardHelp
        }
    }
</script>

<style lang="scss" scoped>
span{
    color: rgb(71, 176, 132);
}
.numbers-p {
    font-size: 13px;
    color: lightgrey;
}

</style>