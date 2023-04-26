<template>
    <div>
        <div class="col  card-wrap" v-for="(card, index) in cards" :key="index">
            <div class="card">
                <div class="card-head text-center">
                    <h3>{{ card.first }}</h3>
                </div>
                <div class="card-body text-center">
                    <p>{{ card.second }}</p>
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
.card{
    padding: 20px;
    width: 300px;
    text-align: center;
    justify-content: center;
    justify-items: center;
}
.card-wrap{
    flex-direction: row;

}

</style>