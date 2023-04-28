<template>
    <div class="d-flex footerR">
        <ul v-for="(list, index) in lists" :key="index" class="footer-links">
                <h6>{{ list.title }}</h6>
                <div class="links">
                    <li v-for="(item, i) in list.links" :key="i">
                    <a :href="item.url">{{ item.text }}</a>
                    </li>
                </div>
            </ul>
    </div>
</template>

<script>
import {rightFooter} from '../assets/data'
    export default {
        name: 'FooterRight',
        data() {
        return {
            lists: rightFooter,
        }
    }
    }
</script>

<style lang="scss" scoped>
ul{
    list-style: none;
}
a{
    text-decoration: none;
    color: rgba(139, 137, 137, 0.853);
}
.footerR{
    margin-left: 300px;
}



</style>