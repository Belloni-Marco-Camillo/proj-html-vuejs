<template>
    <div id="MainSite">
        <HeroSession/>
        <InspiredSession/>
        <SessionBreak/>
        <OurValues/>
        <CtaImg/>
        <TodayNews/>
        <JoingOver/>

    </div>
</template>

<script>
import HeroSession from "./HeroSession.vue";
import InspiredSession from "./InspiredSession.vue";
import OurValues from "./OurValues.vue";
import SessionBreak from "./SessionBreak.vue";
import CtaImg from "./CtaImg.vue";
import TodayNews from "./TodayNews.vue";
import JoingOver from "./JoingOver.vue";

export default {
    components: { HeroSession, InspiredSession, OurValues, SessionBreak, CtaImg, TodayNews, JoingOver }
}
</script>

<style lang="scss">

</style>