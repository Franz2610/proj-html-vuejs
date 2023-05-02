<template>
    <div class="d-flex flex-wrap m-0 p-0">
        <div class="card-wrap" v-for="(card, index) in cards" :key="index">
            <div class="card">
                <div class="card-head text-center">
                    <h3>{{ card.first }}</h3>
                </div>
                <div class="card-body text-center">
                    <p class="fs-6">{{ card.second }}</p>
                    <img :src="card.img" :alt="card.first">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { cardService} from '../assets/data';
    export default {
        name: 'CardService',
        data() {
            return {
                cards: cardService,
            }
        }
    }
</script>

<style lang="scss" scoped>
@use "../assets/partials/variables" as *;

.card{
    width: 270px;
    margin-bottom: 10px;
    border: 0px;
    box-shadow: 3px 1px 1px rgb(115, 115, 115);
}
.card-body{
    box-shadow: 20px;
}
.card-wrap{
    width: 40%;
    height: calc(100% / 2);
}
p{
    color: $bg-g ;
}

</style>