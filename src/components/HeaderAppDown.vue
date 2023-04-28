<template>
    <div class="text-center mt-5 text-white wave">
        <h1>Learn At Your Own Pace!</h1>
        <p>Get teamed uo whit people of the same will</p>
        <button class="btn btn-success py-4"> Get started for free</button>
        <div class="d-flex hero-img">
            <img class="leftperson" src="/public/home-6-hero-left-person.png" alt="left-person">
            <div class="border-img">
                <img class="centerplay" src="/public/video-screen.png" alt="video-screen">
            </div>
            <img class="rightperson" src="/public/home-6-hero-right-person.png" alt="right-person">
        </div>
    </div>
</template>

<script>
    export default {
        name:'HeaderAppDown'
        
    }
</script>

<style lang="scss" scoped>
.wave{
    background-image: url('/public/img/background-pattern-grid-line.png');
    background-image: url('/public/img/jumbotron-background-wave-small.svg');
    background-image: url('/public/img/jumbotron-background-wave-medium.svg');
    background-image: url('/public/img/jumbotron-background-wave-big.svg');
}
.hero-img{
    width: 1000px;
    margin: 100px;
    display: flex;
    justify-content: center;
    align-items: end;
    padding-left: 300px;
    position: absolute;
    background-image: url('/public/img/background-pattern-grid-line.png');
    background-image: url('/public/img/jumbotron-background-wave-small.svg');
    background-image: url('/public/img/jumbotron-background-wave-medium.svg');
    background-image: url('/public/img/jumbotron-background-wave-big.svg');
}
.border-img{
    border: 30px solid white;
    border-radius: 10%;
    z-index: 1000;
}
.centerplay{
        width: 100%;
        z-index: 1000;
        object-fit: contain;
        border-radius: 15px;
        &:hover{
            width: 650px;
            transition: 2s;
            justify-content: center;
        }
    }
.leftperson{
    width: 200px;
    height: 200px;
    position: absolute;
    margin-right: 830px;
    background-image: url('/public/img/background-pattern-grid-line.png');
    background-image: url('/public/img/jumbotron-background-wave-small.svg');
    background-image: url('/public/img/jumbotron-background-wave-medium.svg');
    background-image: url('/public/img/jumbotron-background-wave-big.svg');
}
.rightperson{
    width: 180px;
    height: 120px;
    position: absolute;
    margin-left: 880px;
    margin-top: 20px;
    background-image: url('/public/img/background-pattern-grid-line.png');
    background-image: url('/public/img/jumbotron-background-wave-small.svg');
    background-image: url('/public/img/jumbotron-background-wave-medium.svg');
    background-image: url('/public/img/jumbotron-background-wave-big.svg');
}
button:hover{
    background-color: rgba(56, 56, 173, 0.764);
    color: white;
    transition: 2s;
    padding: 25px;
}
</style>