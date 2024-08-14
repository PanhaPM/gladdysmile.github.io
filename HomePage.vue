<script setup>
        import Slide from './Slider.vue'
        import Scroll from "./Scroll.vue"
        import Recommend2 from './Recommend2.vue';
        import Footer from "./HomePageFooter.vue"
        import Refresh from './Refresh.vue';
        import LeftSlideMenu from './LeftSlideMenu.vue';








           document.addEventListener("DOMContentLoaded", function() {
                var today = new Date();
                var date = (today.getUTCMonth() + 1) + '-' + today.getDate() + '-' +today.getFullYear() ;
                var dateTime = "make today is your day - " + date;  // Ensure the variable name is correct
                document.getElementById("timestamp").innerHTML = dateTime;  // Make sure the ID matches the HTML element
            });
  


</script>


<template>

    <div>
        <!-- refresh -->
    <div class="header">
        <nav>
            <ul>
                <li class="center">
                    <a><LeftSlideMenu /></a>
                </li>
                <li class="center">
                    <a>Brand</a>
                </li>
                <li class="center">
                    <RouterLink to="/ingredient"><a>Ingredient</a></RouterLink>
                </li>
                <li class="center">
                    <RouterLink to="/about"><a>About</a></RouterLink>

                </li>
                <li class="center">
                    <RouterLink to="/"><a><span>GS</span></a></RouterLink>
                </li>                
            </ul>
        </nav>


        <form>
            <div class="search">
                <i class="fa-solid fa-magnifying-glass search-icon"></i>
                <input class="search-input" type="search" placeholder="Search">
            </div>
        </form>
       
        <div class="text-wrapper">
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
            <div>
                <h1>Transform your <span>Skin</span>, <a>Transform your</a> <span>Confident</span><i class="fa-regular fa-face-smile"></i></h1>  
            </div>      
              
               
        </div>
        
        <div class="login-icon">
            <RouterLink to="/login"><a><i class="fa-solid fa-user user"></i></a></RouterLink>
            <RouterLink to="/favourite"><a><i class="fa-solid fa-heart heart"></i></a></RouterLink>
            <RouterLink to="/location"><a><i class="fa-solid fa-location-dot location"></i></a></RouterLink>
            <a><i class="fa-solid fa-dollar-sign usd"></i></a>
            <a><i class="fa-solid fa-bars menu"></i></a>

        </div>


        

        <p id="timestamp"></p>

        <div class="check">
            Check Out The Biggest Trends
        </div>

        <div class="showtext">
            <div class="image">
                <img src="/src/assets/img/spain.png" alt="">
                <div class="content">
                    <p>Spain Kit</p>
                </div>
            </div>
            <div class="image">
                <img src="/src/assets/img/centella.png" alt="">
                <div class="content">
                    <p>Centella</p>
                </div>
            </div>
            <div class="image">
                <img src="/src/assets/img/rolex.jpg" alt="">
                <div class="content">
                    <p>Watches</p>
                </div>
            </div>
            <div class="image">
                <img src="/src/assets/img/argentina.png" alt="">
                <div class="content">
                    <p>Argentina Kit</p>
                </div>
            </div>
            <div class="image">
                <img src="/src/assets/img/mary.jpg" alt="">
                <div class="content">
                    <p>Mary and May</p>
                </div>
            </div>
            <div class="image">
                <img src="/src/assets/img/air-jordan.png" alt="">
                <div class="content">
                    <p>Shoes</p>
                </div>
            </div>
        </div>


        <div class="category">
            <p>Shop by Catetory</p>
        </div>

        <!-- slide -->
        <div style="margin-top:120px;">
            <Slide />
        </div>
        
        <div>
            <Scroll />
        </div>

        <div>
            <div class="Recommend">
                Our Recommend List For You
            </div>
            <Recommend2 />
        </div>


        <RouterLink to="/recommend"><button class="btn1">View More</button></RouterLink>

        <div class="Footer">

            <a href=""><i class="fa-brands fa-facebook facebook"></i></a>
            <a href=""><i class="fa-brands fa-instagram instagram"></i></a>
            <a href=""><i class="fa-brands fa-tiktok tiktok"></i></a>
            <a href=""><i class="fa-brands fa-youtube youtube"></i></a>
            <Footer />

        </div>
     


    </div>
</div>
</template>



<style scoped>
    *{
        padding: 0;
        margin: 0;
        box-sizing: border-box;
        user-select: none;
    }
    .header{
        width: 100%;
        height: 100%;
    }
    .btn1{
        font-size: 20px;
        color: white;
        background-color: black;
        padding-inline: 30px;
        padding-block: 10px;
        border-radius: 50px;
        margin-left: 880px;
        font-weight: 600;
        transition: 0.3s;
    }
    .btn1:hover{
        transform: scale(1.04)
    }
    nav{
        padding: 10px auto;
    }
    nav ul li{
        list-style: none;
        display: inline-block;
        margin: 10px 0px;
        margin-left: 120px;
        margin-top: 80px;
        font-size: 18px;

    }
    nav ul li a{
        position: relative;
        display: block;
        text-decoration: none;
        color: black;
        font-weight: 500;
        cursor: pointer;
        font-size: 18px;
    }
    nav ul li a:before{
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        height: 2.5px;
        width: 0%;
        background: rgb(253, 132, 172);
        border-radius: 12px;
        transition: all 0.4s ease;
    }
    ul li a:hover:before{
        width: 100%;
    }
    ul li.center a:before{
        left: 50%;
        transform: translateX(-50%);
    }
    nav ul li a span{
        font-family: "Playwrite CU", cursive;
        font-optical-sizing: auto;
        font-weight: bold;
        font-style: normal;
        position: absolute;
        text-align: center;
        top: -7px;
        margin-left: 140px;
        font-size: 18px;
        color: palevioletred;
    }


    
    .search{
        position: absolute;
        padding: 8px;
        padding-left: 19px;
        width: max-content;
        display: flex;
        align-items: center;
        padding: var(padding);
        border-radius: 28px;
        background: whitesmoke;
        transition: background 0.25s;
        cursor: pointer;
        float: right;
        margin-top: -45px;
        right: 430px;
    }
    .search:focus-within{
        box-shadow: 0 0 2px rgba(0, 0, 0, 0.75);
    }
    .search-input{
        font-size: 16px;
        font-family: "Lexend", sans-serif;
        color: #333333;
        margin-left: 14px;
        outline: none;
        border: none;
        background: transparent;
        width: 200px;   
    }
    .search-input::placeholder,
    .search-icon{
        color: rgba(0,0,0,0.5);
    }
    
    .text-wrapper{
        width: 100%;
        position: absolute;
        display: flex;
        justify-content: flex-start;
        background-color: whitesmoke;
        overflow: hidden;
        top: 0px;
        padding-block: 10px;
        margin-top: 0;
        padding-inline: 20px;
    }
    h1{
        font-size: 15px;
        letter-spacing: 1px;
        animation: move-rtl 9000ms linear infinite;
        white-space: nowrap;
        font-weight: 500;
        cursor: pointer;
    }
    @keyframes move-rtl{
        0% {
            transform: translateX(0);
        }
        100% {
            transform: translateX(-100%);
        }
    }
    .text-wrapper i{
        padding-inline: 20px;
        font-size: 18px;
    }
    .text-wrapper span{
        font-weight: bold;
        color: palevioletred;
        font-family: "Playwrite CU", cursive;
        font-optical-sizing: auto;
        font-weight: bold;
        font-style: normal;
    }
    .text-wrapper a{
        padding-left: 10px;
    }
    .login-icon{
        position: absolute;
        font-size: 20px;
        color: black;
        top: 73px;
        right: 40px;
        cursor: pointer;
        display: flex;
        justify-content: space-between;
       
    }
    .login-icon a .user {
        color: black;
        margin-left: 60px;
    }
    .login-icon a .heart{
        color: black;
        margin-left: 60px;
    }
    .login-icon a .location{
        color: black;
        margin-left: 60px;
    }
    .login-icon a .usd{
        color: black;
        margin-left: 60px;
        font-weight: bold;
    }
    .login-icon a .menu{
        color: black;
        margin-left: 60px;
        font-weight: bold;
    }
    
    #timestamp{
        font-family: "Playwrite DK Uloopet", cursive;
        font-optical-sizing: auto;
        font-weight: weight;
        font-style: normal;
        text-align: center;
        color: black;
        font-size: 18px;
        padding-top: 130px;
    }
    .check{
        font-family: "Work Sans", sans-serif;
        font-optical-sizing: auto;
        font-weight: weight;
        font-style: normal;
        font-size: 125px;
        font-weight: bold;
        text-align: center;
        margin-top: 30px;
    } 

    /* hsop by catetory */
    .showtext{
        width: 100%;
        height: 100%;
        margin-top: 30px;
        overflow: hidden;
    }
    .image{
        width: 500px;
        position: relative;
        float: left;
        margin-left: 100px;
        margin-top: 20px;
        width: 200px;
        height: 200px;
        border-radius: 100%;
        overflow: hidden;
        object-fit: fill;
        cursor: pointer;
    }
    img{
        width: 100%;
        display: block;
        object-fit: cover;
    }
    .content{
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        position: absolute;
        background: rgba(0, 0, 0, 0.6);
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        opacity: 0;
        transition: 0.6s;
    }
    .content:hover{
        opacity: 1;
        cursor: pointer;
    }
    .content p{
        font-family: "Playwrite DK Loopet", cursive;
        font-optical-sizing: auto;
        font-weight: weight;
        font-style: normal;
        font-size: 25px;
        color: white;
        margin-bottom: 5px;
        cursor: pointer;
    }
    .content > *{
        transform: translateY(25px);
        transition: transform 0.6s;
    }
    .content:hover > *{
        transform: translateY(0px);
    }

    .category p{
        font-family: "Playwrite DK Loopet", cursive;
        font-optical-sizing: auto;
        font-weight: weight;
        font-style: normal;
        color: rgb(223, 122, 155);
        font-size: 80px;
        text-align: center;
        margin-top: 110px;
    }

    /* list brand */

    .img-brand {
        width: 100%;
        height: auto;
    }

    .Recommend{
        font-size: 40px;
        font-weight: bold;
        margin-left: 100px;
        margin-top: 100px;
    }
    .facebook{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 260px;
        margin-left: 680px;
        font-weight: bold;
    }
    .instagram{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 260px;
        margin-left: 855px;
        font-weight: bold;
    }
    .tiktok{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 260px;
        margin-left: 1015px;
        font-weight: bold;
    }
    .youtube{
        position: absolute;
        z-index: 99;
        font-size: 40px;
        color: black;
        cursor: pointer;
        margin-top: 260px;
        margin-left: 1180px;
        font-weight: bold;
    }



</style>    