<template>
    <div class="container ">
        <div class="text-center intestazione align-items-center">
            <h2 class="fs-2"> Let passion and determination be the guide along the way and develop at your own pace that's confortable.</h2>
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
                <div>
                <ul class="text-start">
                    <li><i class="fa-solid fa-angle-down"></i>Select & customize courser to your preferences</li>
                    <li><i class="fa-solid fa-angle-down"></i>Change the tutor and make arrangements</li>
                    <li><i class="fa-solid fa-angle-down"></i>Partecipate in events to join others </li>
                    <li><i class="fa-solid fa-angle-down"></i>Get the desired certificate delivered at house</li>
                </ul>
                </div>
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
@use "../assets/partials/variables" as *;

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
    color: $btn-green;
}
.numbers-p {
    font-size: 13px;
    color: rgb(159, 159, 159);
    margin-left: 25px;
    margin-bottom: 30px;
}
.mar-30{
   // margin-right: 100px;
    margin-top: 200px;
    font-size: 20px;
    width: 800px;
    h2{
        margin-left: 25px;
    }
    ul{
        list-style: none;
        //width: 300px;
    }
    li{
        color: $bg-g;
        //font-size: 14px;
        //margin: 5px;
        //margin-right: 20px;
        
        i{
            color: $btn-green;
        }
    }
}
button:hover{
    background-color: $bg-primary;
    color: white;
    transition: 2s;
    padding: 25px;
}
button{
    margin-left: 28px;
}
.btn-success{
    background-color: $btn-green;
}


</style>