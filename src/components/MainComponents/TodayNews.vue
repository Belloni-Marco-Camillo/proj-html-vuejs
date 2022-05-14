<template>
    <div id="TodayNews">
        <LogoPage/>
        <div class="container pb-5">
            <h2>Today’s Univeristy News</h2>
            <p>Covering Topics From Classes To Politics And Student Organization Events.</p>
            <hr>
            <div class="news-container row justify-content-center gx-5">

                <div 
                    v-for="(post, index) in posts"
                    :key="index"
                    class="news-card col-3"
                    >
                    <img :src="post.img" class="img-fluid">
                    <div class="title-card text-start"><strong>{{post.title}}</strong></div>
                    <div class="meta d-flex">
                        <div class="pruducer text-start">by {{post.producer}} </div><span>&nbsp; &nbsp;</span>
                        <div class="data">{{post.getMonth}}/{{post.getDay}}/{{post.getFullYear}}</div>
                    </div>
                    <div class="readMore text-start">{{post.readmore}}</div>
                </div>

            </div>
        </div>
        
    </div>
</template>


<script>
import state from "@/state";
import LogoPage from "../LogoPage.vue";


export default {
    name: "TodayNews",

    data() {
        return {
            posts: [
                {
                    title: "What do successful grads think you should study?",
                    href: "#",
                    producer: "admin",
                    img:require("@/./assets/img/news_single_post_header_1.jpg"),
                    getFullYear: new Date().getFullYear(),
                    getMonth: new Date().getMonth(),
                    getDay: new Date().getDay(),
                    readmore: "read more >"
                },
                {
                    title: "Former student discusses success in the fashion industry",
                    href: "#",
                    producer: "admin",
                    img:require("@/./assets/img/news_single_post_header_2.jpg"),
                    getFullYear: new Date().getFullYear(),
                    getMonth: new Date().getMonth(),
                    getDay: new Date().getDay(),
                    readmore: "read more >"
                },
                {
                    title: "How do you best prepare for university?",
                    href: "#",
                    producer: "admin",
                    img:require("@/./assets/img/news_single_post_header_3.jpg"),
                    getFullYear: new Date().getFullYear(),
                    getMonth: new Date().getMonth(),
                    getDay: new Date().getDay(),
                    readmore: "read more >"
                },
            ]
        };
    },
    mounted() {
        state.LastPosts=this.posts;
        //console.log(state.LastPosts);
    },
    components: { LogoPage }
}
</script>

<style lang="scss" scoped>

#TodayNews{
    background-color: #e6e6e6;
    hr{
        color: #ffab0b;
        height: 3px;
        width: 200px;
        margin: 20px auto;
    }
    .news-card{
        
        div{
            padding: 3px 0;
            background-color: white;
        }
    }
    .title-card{
        strong{
            color: #ffab0b;
        }
        background-color: white;
    }
    .pruducer{
        color: #ffab0b;
    }
    .readMore{
        color: #ffab0b;
    }
    
}
</style>