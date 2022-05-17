<template>
    <div id="LowHeader">
        <div class="justify-content-between container">
            <div>
                <img src="./../../assets/img/university_logo.png">
            </div>

            <div class="d-flex">
                <div 
                v-for="(item, index) in menuItems" 
                :key="index">
                <div v-if="item.new !== false" class="mx-3 new-header-news">{{item.item}}</div>
                <div v-else-if="item.applay !== false" class="mx-3 new-header-applay">{{item.item}}</div>
                <div v-else class="mx-3">{{item.item}}</div>
                </div>
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
                    item: "home",
                    href: "#",
                    new: true,
                    applay:false
                },
                {
                    item: "about",
                    href: "#",
                    new: false,
                    applay:false
                },
                {
                    item: "courses",
                    href: "#",
                    new: false,
                    applay:false
                },
                {
                    item: "events",
                    href: "#",
                    new: false,
                    applay:false
                },
                {
                    item: "facilities",
                    href: "#",
                    new: false,
                    applay:false
                },
                {
                    item: "news",
                    href: "#",
                    new: false,
                    applay:false
                },
                {
                    item: "admission",
                    href: "#",
                    new: false,
                    applay:true
                },
            ]
        };
    },
    
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/StyleHeader.scss";
</style>