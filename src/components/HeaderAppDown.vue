<template>
    <div class="text-center mt-5 text-white wave">
        <h1>Learn At Your Own Pace!</h1>
        <p>Get teamed uo whit people of the same will</p>
        <button class="btn btn-success py-4"> Get started for free</button>
        <div class="d-flex hero-img">
            <img class="leftperson" src="/home-6-hero-left-person.png" alt="left-person">
            <div class="border-img">
                <img class="center" src="/video-screen.png" alt="video-screen">
                <iframe  class="centerplay" width="420" height="345" src="https://www.youtube.com/watch?v=ElFJ1qcl74U?playlist=tgbNymZ7vqY&loop=1"></iframe>
            </div>
            <img class="rightperson" src="/home-6-hero-right-person.png" alt="right-person">
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

}
.hero-img{
    width: 1000px;
    margin: 100px;
    display: flex;
    justify-content: center;
    align-items: end;
    padding-left: 300px;
    position: absolute;
}
.border-img{
    border: 30px solid white;
    border-radius: 10%;
    z-index: 1000;
}
.center{
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
.centerplay{
        width: 10%;
        height: 10%;
        border-radius: 15px;
        position: absolute;
        background-image: url('/img/icon-youtube-play.png');
        display: none;
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