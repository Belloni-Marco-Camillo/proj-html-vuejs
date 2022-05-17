<template>
    <header>

        <UpHeader/>

        <LowHeader/>
        
    </header>
</template>


<script>
import UpHeader from "./UpHeader.vue";
import LowHeader from "./LowHeader.vue";
export default {
    name: "HeaderSite",
    data() {
        return {

        };
    },
    components: {
    UpHeader,
    LowHeader,
},
}
</script>

<style lang="scss">

</style>