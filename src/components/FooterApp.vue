<template>
<footer>
    <div class="d-flex ">
        <div class="flex-start text-start">
            <h5>Address</h5>
            <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
            <p>+1(305) 547-9909 (9am - 5pm EST, Monday- Friday) </p>
            <p>support@maxcoach.com</p>
            <div class="me-sm-5">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter mx-4"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin"></i>
            </div>
        </div>
        <div class="flex-end">
            <FooterRight/>
        </div>
    </div>
    <p class="text-center">2020 Maxcoach, All Right Reserved</p>
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

</style>