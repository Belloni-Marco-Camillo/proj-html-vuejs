<template>
    <div id="UpHeader">
        <div class="d-flex container-upheader container justify-content-between align-items-center" >
            <div class="d-flex">

                <div 
                v-for="(item, index) in menuItems" 
                :key="index"
                class="mx-3">
                <a :href="item.href">
                    {{item.item}}
                </a>
                </div>

            </div>

            <div class="d-flex">

                <div
                v-for="(social, index) in SocialIcon" 
                :key="index"
                class="mx-3"><img :src="social.Image"></div>

            </div>

        </div>
        
    </div>
</template>

<script>

export default {
    name: "UpHeader",
    data() {
        return {
            menuItems: [
                {
                    item: "1.800.567.8910",
                    href: "#",
                },
                {
                    item: "Contat Us",
                    href: "#",
                },
                {
                    item: "Alunni",
                    href: "#",
                },
                {
                    item: "Campus",
                    href: "#",
                },
            ],
            SocialIcon:[
                {
                    Image:require("@/./assets/img/icon/facebook.svg"),
                    href:"#"
                },
                {
                    Image:require("@/./assets/img/icon/twitter.svg"),
                    href:"#"
                },
                {
                    Image:require("@/./assets/img/icon/youtube.svg"),
                    href:"#"
                },
                 {
                    Image:require("@/./assets/img/icon/instagram.svg"),
                    href:"#"
                },
            ],
        };
        
    },
}
</script>

<style lang="scss">
@import "@/assets/scss/StyleHeader.scss";
</style>