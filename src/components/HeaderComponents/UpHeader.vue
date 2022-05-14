<template>
    <div id="UpHeader">
        <div class="d-flex container justify-content-between align-items-center" >
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
                class="mx-3">{{social.item}}</div>

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
                    item:"facebook",
                    href:"#"
                },
                {
                    item:"twitter",
                    href:"#"
                },
                {
                    item:"youtube",
                    href:"#"
                },
                 {
                    item:"instagram",
                    href:"#"
                },
            ]
        };
    },
}
</script>

<style lang="scss">
#UpHeader{
    height: 36px;
    background-color: #ffab0b;
    a{
        text-decoration: none;
        color: white;

    }
}
</style>