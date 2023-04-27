<template>
    <div class="d-flex flex-wrap">
        <div class=" d-flex card-wrap" v-for="(card, index) in cards" :key="index">
            <div class="d-flex card-d">
                <div>
                    <img :src="card.img" :alt="card.first">
                </div>
                <div class="text-start">
                    <h4> $ {{ card.price }} </h4>
                    <p>{{ card.name }} </p>
                    <div class="d-flex  number">
                        <p class="m-2"> <i class="fa-solid fa-file-lines"></i> {{ card.lesson }} Lessons</p>
                        <p class="m-2"> <i class="fa-regular fa-user"></i> {{ card.students }} Students</p>
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
h4{
    color: rgb(71, 176, 132);
}
.number {
    font-size: 13px;
    color: rgba(172, 167, 167, 0.853);
}
.card-d:hover{
    background-color: white;
    transition: 1s;
}
</style>