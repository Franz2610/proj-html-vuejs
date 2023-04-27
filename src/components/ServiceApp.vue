<template>
    <div class="container mt-5">
        <div class="text-center intestazione align-items-center">
            <h5 class="strong fs-2"> Let passion and determination be the guide along the way and develop at your own pace that's confortable.</h5>
            <h6 class="mt-3">Funnie Moreno</h6>
            <p class="mt-1">/Founder & CEO</p>
        </div>
        <div class="d-flex text-center justify-content-center align-items-center gap-5 mb-5">
            <ul v-for="(num, index) in nums" :key="index" class=" text-center justify-content-center align-items-center gap-1">
               <h2 class="m-0 text-uppercase d-flex text-center"><span>{{ num.first }}</span></h2>
               <p class="m-0 text-uppercase d-flex  numbers-p">{{ num.second }}</p>
            </ul>
        </div>
        <div class="d-flex card-wrapper">
            <div>
                <CardService/>
            </div>
            <div class="mar-30">
                <p class="text-uppercase  numbers-p">togheter we can create</p>
                <h2>Service We <span>Can Provide</span>  For My Clients.</h2> 
                <ul class="text-start">
                    <li><i class="fa-solid fa-angle-down"></i>Select & customize courser to your preferences</li>
                    <li><i class="fa-solid fa-angle-down"></i>Change the tutor and make arrangements</li>
                    <li><i class="fa-solid fa-angle-down"></i>Partecipate in events to join others </li>
                    <li><i class="fa-solid fa-angle-down"></i>Get the desired certificate delivered at house</li>
                </ul>
                <button class="btn btn-success">Get started for free</button>
            </div>
        </div>
    </div>
</template>

<script>
import { numService } from '../assets/data';
import CardService from './CardService.vue'
    export default {
        name: 'ServiceApp',
        components:{
            CardService,
        },
        data() {
            return {
                nums: numService,
            }
        }
    }
</script>

<style lang="scss" scoped>
/*.card-wrapper{
    height: 650px;
}*/
.intestazione{
    width: 650px;
    height: 380px;
    margin-left: 300px;
    margin-top: 200px;
    p{
        color: lightgrey;
        font-size: 10px;
    }
    
}
span{
    color: rgb(71, 176, 132);
}
.numbers-p {
    font-size: 13px;
    color: lightgrey;
}
.mar-30{
    margin-right: 100px;
    margin-top: 200px;
    font-size: 20px;
    ul{
        list-style: none;
    }
    li{
        color: lightgrey;
        font-size: 14px;
        margin: 5px;
        
        i{
            color: rgb(71, 176, 132);
        }
    }
}

</style>