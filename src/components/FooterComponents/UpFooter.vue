<template>
    <div id="UpFooter">
        <div class="container-footer d-flex align-items-center justify-content-around">

            <div >

                <div
                    v-for="(item, index) in FooterItems" 
                    :key="index">
                        <div>{{item.conctat}}</div>
                        <div>{{item.road}}</div>
                        <div>{{item.state}}</div>
                </div>

            </div>

            <div>

                <div
                    v-for="(item, index) in FooterPost"
                    :key="index">
                    <div>{{item.title}}</div>
                </div>

            </div>


        </div>
        
        
    </div>
</template>

<script>
import state from "@/state";
export default {
    name: "UpFooter",
    data() {
        return {
            FooterPost:[],
            FooterItems: [
                {
                    conctat: "Residential Location",
                    road: "9521 Broadsberry Avenue",
                    state: "Paddington RC7 9ZA",
                },
                {
                    conctat: "1.800.458.556",
                },
                {
                    conctat: "info@your-domain.com",
                },
                {
                    conctat: "Monday – Friday: 8:00 AM – 10:00 PM"
                },
            ]
        };
    },
    mounted() {
        this.FooterPost=state.LastPosts;  
        console.log(this.FooterPost);
    },
}
</script>

<style lang="scss">
#UpFooter{
    height: 425px;
    background-image: url(./../../assets/img/university_ft_bg.png);
    background-position: center;
    .container-footer{
        height: 100%;
    }
}
</style>