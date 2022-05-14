<template>
    <div id="CtaImg">
        <div class="row">
            <div class="col-4 d-flex flex-column align-items-center justify-content-center">
                <h2>
                    courses
                </h2>
                <hr>
                <p><a href="#"> view more</a></p>
            </div>
            <div class="col-4 d-flex flex-column align-items-center justify-content-center">
                <h2>
                    events
                </h2>
                <hr>
                <p><a href="#"> view more</a></p>
            </div>
            <div class="col-4 d-flex flex-column align-items-center justify-content-center">
                <h2>
                    lastest news
                </h2>
                <hr>
                <p><a href="#"> view more</a></p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
#CtaImg{
    height: 65vh;
    .row{
        height: 100%;
        background-size: cover;
        background-position: top;
        background-repeat: no-repeat;
        h2{
            color: white;
            text-transform: uppercase;
        }
        hr{
            height: 2px;
            color: #ffab0b;
            width: 80px;
        }
        a{
            color: white;
            text-decoration: none;
        }
        div:nth-child(1){
            background-image: url(./../../assets/img/home_courses_section_bg.jpg);
        }
        div:nth-child(2){
            background-image: url(./../../assets/img/home_events_section_bg.jpg);
        }
        div:nth-child(3){
            background-image: url(./../../assets/img/home_latest_news_section_bg.jpg);
        }
    }
}
</style>