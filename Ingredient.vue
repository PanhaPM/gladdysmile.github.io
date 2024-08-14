<script setup>
    import {ref} from 'vue'
    import {itemList} from "./Store"
    const slideInd = ref(0)
    const nextSlide = () => {
        slideInd.value++
        if(slideInd.value >= itemList.value.length){
            slideInd.value=0
        }
    }
    const backSlide = () => {
        slideInd.value--
        if(slideInd.value<0){
            slideInd.value = itemList.value.length-1
        }
    }
    const clickSlide = (i) => {
        slideInd.value = i
    }
    var autoSlide = setInterval( nextSlide, 1000 )
    const stopAutoSlide = () => {
        clearInterval(autoSlide)
    }
    const runAutoSlide = () => {
        autoSlide = setInterval( nextSlide, 1000 )
    }
</script>

<template>
    <div class="col-xxl-9 col-xl-9 slide-container">
        <div class="slide-box" @mouseover="stopAutoSlide" @mouseleave="runAutoSlide">
            <ul class="pagination">
                <li 
                v-for="(item,i) in itemList" :key="i" :class="{'active': i==slideInd}" @click="clickSlide(i)"> {{ i+1 }} 
                </li>
            </ul>
            <div class="slide" v-for="(item, i) in itemList" :key="i" v-show="i==slideInd">
                <img :src="item.img" alt="">
            </div>
            <div class="btnSlide btn-next" @click="nextSlide" >
                Next
            </div>
            <div class="btnSlide btn-back" @click="backSlide">
                Back
            </div>

            
        </div>
        <div class="title"><p>Natural Ingredients</p></div>
            <div class="ingredients">
            <div class="ingredient"><a href="#">Centella Asiatica</a></div>
            <div class="ingredient"><a href="#">Houttuynia Cordata</a></div>
            <div class="ingredient"><a href="#">Tea Tree</a></div>
            <div class="ingredient"><a href="#">Marine Collagen</a></div>
            <div class="ingredient"><a href="#">Blackberry Complex</a></div>
            <div class="ingredient"><a href="#">Chaenomeles</a></div>
            <div class="ingredient"><a href="#">Citrus Unshiu Fruit</a></div>
            <div class="ingredient"><a href="#">Tremella Fuciformis</a></div>
            <div class="ingredient"><a href="#">Betula Alba Juice</a></div>
            <div class="ingredient"><a href="#">Damask Rose Water</a></div>
            <div class="ingredient"><a href="#">Bakuchiol</a></div>
            <div class="ingredient"><a href="#">Jojoba Seed Oil</a></div>
            <div class="ingredient"><a href="#">Red Grape Extract</a></div>
            <div class="ingredient"><a href="#">Witch Hazel Extract</a></div>
            <div class="ingredient"><a href="#">Calendula Extract</a></div>
            <div class="ingredient"><a href="#">Pomegranate Extract</a></div>
        </div>

            
        <div class="title-2"><p>Pure Ingredients</p></div>
            <div class="ingredients-2">
            <div class="ingredient"><a href="#">Peptide</a></div>
            <div class="ingredient"><a href="#">Idebenone</a></div>
            <div class="ingredient"><a href="#">Hyaluronics</a></div>
            <div class="ingredient"><a href="#">Niacinamide</a></div>
            <div class="ingredient"><a href="#">Panthenol</a></div>
            <div class="ingredient"><a href="#">Chaenomeles</a></div>
            <div class="ingredient"><a href="#">Gluconolactone</a></div>
            <div class="ingredient"><a href="#">Ceramide</a></div>
            <div class="ingredient"><a href="#">Bifida</a></div>
            <div class="ingredient"><a href="#">Tranexamic acid</a></div>
            <div class="ingredient"><a href="#">Glutathione</a></div>
            <div class="ingredient"><a href="#">Vitamin C</a></div>
            <div class="ingredient"><a href="#">Allantoin</a></div>
            <div class="ingredient"><a href="#">Kaoline</a></div>
            <div class="ingredient"><a href="#">Phyto sphingosine</a></div>
            <div class="ingredient"><a href="#">sphingosine</a></div>
        </div>









        <div style="margin-top:210px;padding:15px 15px 2500px;font-size:30px"></div>
    </div>
</template>

<style scoped>
    .slide-container{
        width: 100%;
        height: 911px;
    }
    .slide-box{
        width: 100%;
        height: 100%;
        background-color: white;
        display: flex;
        position: relative;
        gap: 6px;
    }
    .slide-box ul{
        position: absolute;
        bottom: 9px;
        left: 50%;
        transform: translate(-50%, 0);
        background-color: rgba(44, 43, 43, 0.172);
        padding: 6px;
        border-radius: 6px;
        display: flex;
        gap: 9px;
        z-index: 1;
    }
    .slide-box ul li{
        width: 25px;
        height: 25px;
        border-radius: 50%;
        background-color: white;
        color: black;
        font-size: 12px;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
    }
    .slide-box ul li.active{
        background-color: seagreen;
        color: white;
    }
    .slide-box ul li:hover{
        background-color: seagreen;
        color: white;
    }
    .slide-box .slide{
        width: 100%;
        height: 100%;
        position: relative;
    }
    .slide-box .slide span{
        position: absolute;
        top: 6px;
        left: 6px;
        background-color: rgba(46, 139, 86, 0.693);
        color: white;
        font-size: 15px;
        padding: 9px;
        border-radius: 9px;
    }
    .slide-box .slide img{
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    .btnSlide{
        position: absolute;
        top: 50%;
        transform: translate(0, -50%);
        padding: 9px 18px;
        background-color: seagreen;
        color: white;
        cursor: pointer;
        border-radius: 6px;
        box-shadow: 1px 1px 3px dimgray;
    }
    .btn-next{
        right: 30px;
    }
    .btn-back{
        left: 30px;
    }
    .title{
        position: relative;
        margin-top: 200px;
        background-color: #F3F3F3;
        align-content: center;
        height: 65px;
        width: 1180px;
        margin-left: 360px;
        margin-bottom: 40px;
    }
    .title p{
        position: absolute;
        font-size: 35px;
        color: black;
        text-align: center;
        width: 30%;
        padding-inline: 0;
        align-content: center;
        margin-left: 440px;
        margin-top: -33px;
        z-index: 2;
    }
    .ingredients {
        display: flex;
        flex-wrap: wrap;
        max-width: 1140px;
        margin: auto;
        font-family: Arial, sans-serif;
        justify-content: space-between;
        text-decoration: none;
    }
    .ingredient {
        color: #bbb;
        font-size: 21px;
        width: calc(25% - 20px); /* Adjust this value for better spacing */
        padding: 10px 0;
        text-align: center;
    }
    .ingredient a {
        text-decoration: none;
        color: gray;
    }
    .ingredient a:hover{
        color: palevioletred;
    }




    .title-2{
        position: relative;
        margin-top: 120px;
        background-color: #F3F3F3;
        align-content: center;
        height: 65px;
        width: 1180px;
        margin-left: 360px;
        margin-bottom: 40px;
    }
    .title-2 p{
        position: absolute;
        font-size: 35px;
        color: black;
        text-align: center;
        width: 30%;
        padding-inline: 0;
        align-content: center;
        margin-left: 440px;
        margin-top: -33px;
        z-index: 2;
    }
    .ingredients-2 {
        display: flex;
        flex-wrap: wrap;
        max-width: 1140px;
        margin: auto;
        font-family: Arial, sans-serif;
        justify-content: space-between;
        text-decoration: none;
    }
    .ingredient {
        color: #bbb;
        font-size: 21px;
        width: calc(25% - 20px); /* Adjust this value for better spacing */
        padding: 10px 0;
        text-align: center;
    }
    .ingredient a {
        text-decoration: none;
        color: gray;
    }
    .ingredient a:hover{
        color: black;
    }
        
</style>