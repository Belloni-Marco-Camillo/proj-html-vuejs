<template>
    <div id="JoingOver">
        <div class="container-cta-news container d-flex flex-column justify-content-center align-items-center">
            <h2>Joing Over <span>500,000 Students</span>  Enjoying Avada Education now</h2>
            <p>Become Part of Avada University to Further Your Career.</p>
            <div class="d-flex">
                <input type="text" placeholder="Name">
                <input type="text" placeholder="Email">
                <input type="text" placeholder="Telephone">
                <button>apply now</button>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
#JoingOver{
    height: 290px;
    background-color: #333C4E;
    color: white;
    span{
        color:#ffab0b;
    }
    p{
        color: #7b7e85;
    }
    input{
        background-color: #667287;
        border: none;
        margin: 0 5px;
        padding: 5px 0;
        color: white;
    }
    button{
        margin-left:5px ;
        background-color: #ffab0b;
        border: none;
        color: white;
        padding: 5px 20px;
        text-transform: uppercase;
        
    }
    .container-cta-news{
        height: 100%;
    }
}
</style>