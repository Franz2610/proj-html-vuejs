<template>
    <div class="text-center mt-5 text-white">
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
    width: 1000px;
    margin: 100px;
    display: flex;
    justify-content: center;
    align-items: end;
    padding-left: 300px;
    position: absolute;
}
.centerplay{
        width: 100%;
        z-index: 1000;
    }
.leftperson{
    width: 200px;
    height: 200px;
    position: absolute;
    margin-right: 830px;
}
.rightperson{
    width: 180px;
    height: 120px;
    position: absolute;
    margin-left: 880px;
    margin-top: 20px;
}
button:hover{
    background-color: rgba(56, 56, 173, 0.764);
    color: white;
    transition: 2s;
    padding: 25px;
}
</style>