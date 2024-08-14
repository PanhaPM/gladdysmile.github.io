<template>
    <div class="header">
        <div class="background">
            <i class="fa-solid fa-heart heart"></i>
            <div class="title">
                Your Favourite List Is Empty Now
            </div>
            <p>But doesn't have to be. Add items by clicking on the heart as you browse around.</p>
            <button>Add Now</button>
        </div>
        <div class="name">You can add some favourite on here</div>
        <div><ListShop4Favourite /></div>

        <a href=""><i class="fa-brands fa-facebook facebook"></i></a>
        <a href=""><i class="fa-brands fa-instagram instagram"></i></a>
        <a href=""><i class="fa-brands fa-tiktok tiktok"></i></a>
        <a href=""><i class="fa-brands fa-youtube youtube"></i></a>
        <div class="footer"><Footer />
        </div>
    </div>
</template>

<style scoped>
    *{
        padding: 0;
        margin: 0;
        box-sizing: border-box;
    }
    .header{
        width: 100%;
        height: 100%;
    }
    .background{
        background-color: whitesmoke;
        width: 100%;
        height: 550px;
    }
    .heart{
        font-size: 100px;
        color: black;
        margin-left: 900px;
        margin-top: 180px;
    }
    .title{
        font-size: 33px;
        color: black;
        font-weight: bold;
        margin-left: 690px;
        margin-top: 40px;
    }
    p{
        font-size: 17px;
        margin-left: 632px;
        margin-top: 10px;
        font-weight: 500;
    }
    button{
        font-size: 17px;
        border: none;
        border-radius: 50px;
        background-color: black;
        font-weight: bold;
        color: white;
        padding-block: 10px;
        padding-inline: 40px;
        margin-left: 875px;
        margin-top: 30px;
        transition: 0.3s;
    }
    button:hover{
        -ms-transform: scale(1.05);
        -webkit-transform: scale(1.05); 
        transform: scale(1.05); 
    }
    .name{
        font-size: 38px;
        font-weight: bold;
        margin-top: 70px;
        margin-left: 100px;
    }
    .footer{
        margin-top: 600px;
    }
    .facebook{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 280px;
        margin-left: 680px;
        font-weight: bold;
    }
    .instagram{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 280px;
        margin-left: 855px;
        font-weight: bold;
    }
    .tiktok{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 280px;
        margin-left: 1015px;
        font-weight: bold;
    }
    .youtube{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 280px;
        margin-left: 1180px;
        font-weight: bold;
    }
</style>

<script setup>
    import ListShop4Favourite from './ListShop4Favourite.vue';
    import Footer from "./Footer.vue"
</script>