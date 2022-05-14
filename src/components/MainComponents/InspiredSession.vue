<template>
    <div id="InpiredSession" class="container mt-5 mb-5">
        <LogoPage/>
        <div class="headertext">
            <h2>Inspired By Excellence & Innovation</h2>
            <p>We Offer A Wide Range Of High Quality Of Teaching And Extra-Curricular Activities.</p>
            <hr>
        </div>

        <div class="row mt-5 align-items-end">
            <div class="col-7 text-start">
                <h3>WHY CHOOSE AVADA UNIVERSITY</h3>
                <p>
                    We offer a range of training packages in a range of subject areas and can offer blended learning opportunities to best meet your needs. 
                    If sitting in a room with a trainer and having the opportunity for discussion with other learners sounds good to you then we can offer this. 
                    If you prefer to study in your own time and at your own speed then one of our world class facilities.
                </p>
                <p>
                    If you prefer to study in your own time and at your own speed then one of our e-learning packages may be right up your street. 
                    There is a third option, which is you like the sound of both but perhaps can’t attend all training sessions, 
                    this is when blended learning comes into its own.
                </p>
            </div>
            <div class="col-5">
                <iframe title="vimeo-player" src="https://player.vimeo.com/video/80567526?h=1334ac0d68" width="340" height="190" frameborder="0" allowfullscreen></iframe>
            </div>
        </div>
    
        
    </div>
    
</template>

<script>
import LogoPage from "../LogoPage.vue";

export default {
    components: { LogoPage }
}
</script>

<style lang="scss" scoped>

.headertext{
    hr{
        color: #ffab0b;
        height: 3px;
        width: 150px;
        margin: 0 auto;
    }
    
}

</style>