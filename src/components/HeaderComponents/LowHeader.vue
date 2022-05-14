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
                <div class="mx-3">{{item.item}}</div>
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
                    new: false,
                },
                {
                    item: "about",
                    href: "#",
                    new: false,
                },
                {
                    item: "courses",
                    href: "#",
                    new: false,
                },
                {
                    item: "events",
                    href: "#",
                    new: false,
                },
                {
                    item: "facilities",
                    href: "#",
                    new: false,
                },
                {
                    item: "news",
                    href: "#",
                    new: false,
                },
                {
                    item: "admission",
                    href: "#",
                    new: false,
                },
            ]
        };
    },
    
}
</script>

<style lang="scss" scoped>
#LowHeader{
    height: 90px;
    div{
        height: 100%;
        display: flex;
        align-items: center;
    }
    img{
        height: 50px;
    }
}
</style>