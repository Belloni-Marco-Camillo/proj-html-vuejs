<template>
    <div id="HeroSession" class="d-flex justify-content-center align-items-center">

        <div>
            <h1>Inspiriting Tomorrow Leaders</h1> 
        
            <h4>The Future Belongs To Those Who See Possibilies Today</h4>

            <div class="mt-4 d-flex justify-content-center">
                <button class="find border-0">find a course</button>
                <button class="apply border-0">apply now</button>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
#HeroSession{
    height: 80vh;
    background-image: url(./../../assets/img/home_main_slider_bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    color: white;
    button{
        text-transform: uppercase;
        margin: 0 10px 0 10px;
        padding: 10px 20px 10px 20px;
        color: white;
        
    }
    .find{
        
        background-color: #ffab0b;
    }
    .apply{
        background-color: #77e6fe;
    }
}
</style>