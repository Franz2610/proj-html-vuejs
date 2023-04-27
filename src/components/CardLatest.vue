<template>
    <div class="d-flex">
        <div class=" d-flex card-wrap" v-for="(card, index) in cards" :key="index">
            <div class="text-start">
                    <img :src="card.img" :alt="card.name">
                    <p>{{ card.role }}</p>
                    <h4>{{ card.name }}</h4>
                    <div class="d-flex text-start">
                        <p class="m-2"> <i class="fa-regular fa-calendar"></i>{{ card.date }}</p>
                        <p class="m-2"> <i class="fa-solid fa-eye"></i>{{ card.views }}</p>
                    </div>                
            </div>
        </div>
    </div>
</template>

<script>
import { cardLatest} from '../assets/data';
    export default {
        name: 'CardService',
        data() {
            return {
                cards: cardLatest,
            }
        }
    }
</script>

<style lang="scss" scoped>
.card-wrap{
    width: calc(100% / 2);
    margin-top: 100px;
}

img{
    width: 90%;
}

</style>