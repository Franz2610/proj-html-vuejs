<template>
    <div class="d-flex">
        <div class="  card-wrap" v-for="(card, index) in cards" :key="index">
            <div>
                <div>
                    <img :src="card.img" :alt="card.first">
                </div>
                <div class="paragraph">
                    <h5>{{ card.first }}</h5>
                    <p>{{ card.second }}</p>
                </div>
                
            </div>
        </div>
    </div>
</template>

<script>
import { cardHelp} from '../assets/data';
    export default {
        name: 'CardHelp',
        data() {
            return {
                cards: cardHelp,
            }
        }
    }
</script>

<style lang="scss" scoped>
.card-wrap{
    width: calc(100% / 4);
}

img{
    width: 50%;
    //height: 70%;
}
.paragraph{
    width: 300px;
}

</style>