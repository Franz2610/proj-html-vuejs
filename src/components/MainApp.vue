<template>
    <main>
        <ServiceApp/>
        <FeaturesApp/>
        <TalkAbout/>
        <LatestApp/>
        <HelpApp/>
        <BtnApp/>
    </main>
</template>

<script>
import ServiceApp from './ServiceApp.vue';
import FeaturesApp from './FeaturesApp.vue';
import TalkAbout from './TalkAbout.vue';
import LatestApp from './LatestApp.vue';
import HelpApp from './HelpApp.vue';
import BtnApp from './BtnApp.vue';
    export default {
        name: 'MainApp',
        components:{
            ServiceApp,
            FeaturesApp,
            TalkAbout,
            LatestApp,
            HelpApp,
            BtnApp
        }
    }
</script>

<style lang="scss" scoped>

</style>