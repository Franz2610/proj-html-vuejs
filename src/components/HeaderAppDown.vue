<template>
    <div class="text-center">
        <h1>Learn At Your Own Pace!</h1>
        <p>Get teamed uo whit people of the same will</p>
        <button class="btn btn-success py-4"> Get started for free</button>
        <div class="d-flex hero-img">
            <img class="leftperson" src="../../public/home-6-hero-left-person.png" alt="left-person">
            <img class="centerplay" src="../../public/video-screen.png" alt="video-screen">
            <img class="rightperson" src="../../public/home-6-hero-right-person.png" alt="right-person">
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.hero-img{
    width: 800px;
    margin: 100px;
    display: flex;
    justify-content: center;
    align-items: end;
}
.centerplay{
        width: 100%;
    }
.leftperson, .rightperson{
    width: 150px;
    height: 150px;

}
</style>