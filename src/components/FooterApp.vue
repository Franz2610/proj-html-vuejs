<template>
<footer>
    <div class="d-flex container">
        <div class="flex-start text-start">
            <h5>Address</h5>
            <p class="numbers">382 NE 191st St # 87394 Miami, FL 33179-3899</p>
            <p class="numbers">+1(305) 547-9909 (9am - 5pm EST, Monday- Friday) </p>
            <p class="numbers">support@maxcoach.com</p>
            <div class="me-sm-5 numbers">
                <i class="fa-brands fa-facebook-f mx-1 "></i>
                <i class="fa-brands fa-twitter mx-1"></i>
                <i class="fa-brands fa-instagram mx-1"></i>
                <i class="fa-brands fa-linkedin mx-1"></i>
            </div>
        </div>
        <div class="flex-end">
            <FooterRight/>
        </div>
    </div>
    <p class="text-center number">2020 Maxcoach, All Right Reserved</p>
</footer>
</template>

<script>
import FooterRight from './FooterRight.vue';
    export default {
        name:'FooterApp',
        components:{
            FooterRight
        }
        
    }
</script>

<style lang="scss" scoped>
.number {
    font-size: 13px;
    color: rgba(172, 167, 167, 0.853);
}
.numbers{
    color: rgba(139, 137, 137, 0.853);
}


</style>