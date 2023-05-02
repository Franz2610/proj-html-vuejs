<template>
    <div class="text-center mt-5 container mb-5">
        <h3>Why People Talk About <span> MaxCoach</span> ?</h3>
        <div class="d-flex caption-wrapper">
            <div class="img-shape">
                <img class="shape" src="../../public/img/maxcoach-shape-05.png" alt="shape">
                <img class="img-header m-5" src="../../public/img/testimonial-avata-02.jpg" alt="testimonial2">
            </div>
            <div class="captions text-start">
                <p class="fs-3">I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
                <h6 class="text-uppercase">mina hollage</h6>
                <p>/Freelancer</p>
            </div>
        </div>
        <div class="d-flex img-wrapper">
            <img class="m-5" src="/public/img/client-logo-colored-01.png" alt="logoclient-1">
            <img class="m-5" src="/public/img/client-logo-colored-02.png" alt="logoclient-2">
            <img class="m-5" src="/public/img/client-logo-colored-03.png" alt="logoclient-3">
            <img class="m-5" src="/public/img/client-logo-colored-04.png" alt="logoclient-4">
            <img class="m-5" src="/public/img/client-logo-colored-05.png" alt="logoclient-5">
            <img class="m-5" src="/public/img/client-logo-colored-06.png" alt="logoclient-6">
        </div>
    </div>
</template>

<script>
    export default {
        name:'TalkAbout'
    }
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;

.img-wrapper{
    width: 100%;
    height: 80%;
    img{
        width: 70%;
        height: 50%;
    }
}
.img-header{
    border-radius: 50%;
    position: relative;
}
.captions{
    width: 70%;
    height: 60%;
}
.caption-wrapper{
    margin-left: 250px;
    margin-top: 60px;
}
span{
    color: $btn-green;
}
.img-shape{
    position: relative;
}
.shape{
    position: absolute;
    margin-right: 1300px;
}

</style>