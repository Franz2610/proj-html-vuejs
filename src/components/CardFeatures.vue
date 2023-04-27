<template>
    <div class="d-flex flex-wrap">
        <div class=" d-flex card-wrap" v-for="(card, index) in cards" :key="index">
            <div class="d-flex">
                <div>
                    <img :src="card.img" :alt="card.first">
                </div>
                <div class="">
                    <p>{{ card.price }}</p>
                    <p>{{ card.name }}</p>
                    <div class="d-flex tex-center align-items-center justify-content-center number">
                        <p class="m-2"> <i class="fa-solid fa-file-lines"></i> {{ card.lesson }}</p>
                        <p class="m-2"> <i class="fa-regular fa-user"></i>{{ card.students }}</p>
                    </div>
                </div>
                
            </div>
        </div>
    </div>
</template>

<script>
import { cardFeutures} from '../assets/data';
    export default {
        name: 'CardService',
        data() {
            return {
                cards: cardFeutures,
            }
        }
    }
</script>

<style lang="scss" scoped>
.card-wrap{
    width: calc(100% / 2);
}

img{
    width: 70%;
    height: 70%;
    border-radius: 50%;
}

</style>