<template>
    <div id="LowFooter">
        
    
            <div class="d-flex align-items-center justify-content-between contain-lowfooter">

                <div>
                    © Copyright 2012 - 2022 | Avada Theme by <span>ThemeFusion</span> | All Rights Reserved | Powered by <span>WordPress</span>
                </div>

                <div class="d-flex">
                    <div
                        v-for="(social, index) in FooterIcon" 
                        :key="index"
                        class="mx-3"><img :src="social.Image">
                    </div>
                </div>
                

        </div>
    </div>
</template>

<script>

export default {
    name: "LowFooter",
    data() {
        return {
            FooterIcon:[
                {
                    Image:require("@/./assets/img/icon/facebook-grey.svg"),
                    href:"#"
                },
                {
                    Image:require("@/./assets/img/icon/twitter-grey.svg"),
                    href:"#"
                },
                {
                    Image:require("@/./assets/img/icon/youtube-grey.svg"),
                    href:"#"
                },
                 {
                    Image:require("@/./assets/img/icon/instagram-grey.svg"),
                    href:"#"
                },
            ],
        };
    },
}
</script>

<style lang="scss">
#LowFooter{
    height: 75px;
    .contain-lowfooter{
        height: 100%;
        width: 93%;
        margin: 0 auto;
    }
    img{
        height: 15px;
    }
    span{
       color: #ffab0b; 
    }
}
</style>