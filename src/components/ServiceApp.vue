<template>
    <div>
        <div class="text-center">
            <p class="strong"> Let passion and determination be the guide along the way and develop at your own pace that's confortable.</p>
            <h5>Funnie Moreno</h5>
            <h6>/Founder & CEO</h6>
        </div>
        <div class="d-flex text-center justify-content-center align-items-center gap-5">
            <ul v-for="(num, index) in nums" :key="index" class=" text-center justify-content-center align-items-center gap-1">
               <p class="m-0 text-uppercase d-flex fs-5">{{ num.first }}</p>
               <p class="m-0 text-uppercase d-flex fs-5">{{ num.second }}</p>
            </ul>
        </div>
        <div class="d-flex card-wrapper">
            <div>
                <CardService/>
            </div>
            <div>
                <p class="text-uppercase">togheter we can</p>
                <h3>Service We Can Provide For My Clients</h3>
                <ul>
                    <li>Select and customize</li>
                    <li>Change the tutor</li>
                    <li>Partecipate in events</li>
                    <li>Get the desired</li>
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

</style>