<script>
import Recommend2 from './Recommend2.vue';

export default {
  components: { Recommend2 },
  data() {
    return {
      tabs: ['Description', 'Ingredients', 'FAQ', 'How to Use'],
      activeTab: 'Ingredients',
      ingredients: `Water, Oryza Sativa (Rice) Extract (30%), Dibutyl Adipate, Propanediol,
                    Diethylamino Hydroxybenzoyl Hexyl Benzoate, Polymethylsilsesquioxane,
                    Ethylhexyl Triazone, Niacinamide, Methylene Bis-benzotriazolyl
                    Tetramethylbutylphenol, Coco-caprylate/Caprate, Caprylyl Methicone,
                    Diethylhexyl Butamido Triazone, Glycerin, Butylene Glycol, Oryza Sativa
                    (Rice) Germ Extract, Camellia Sinensis Leaf Extract,
                    Lactobacillus/Pumpkin Ferment Extract, Bacillus/Soybean Ferment
                    Extract, Saccharum Officinarum (Sugarcane) Extract, Macrocystis Pyrifera
                    (Kelp) Extract, Cocos Nucifera (Coconut) Fruit Extract, Panax Ginseng
                    Root Extract, Camellia Sinensis Leaf Extract, Monascus/Rice Ferment,
                    Pentylene Glycol, Behenyl Alcohol, Poly C10-30 Alkyl Acrylate,
                    Polyglyceryl-3 Methylglucose Distearate, Decyl Glucoside,
                    Tromethamine, Carbomer, Acrylates/C10-30 Alkyl Acrylate
                    Crosspolymer, 1,2-Hexanediol,Sodium Stearoyl Glutamate, Polyacrylate
                    Crosspolymer-6, Ethylhexylglycerin, Adenosine, Xanthan Gum,
                    Tocopherol, Lactobacillus/Rice Ferment, Aspergillus Ferment,
                    Saccharomyces/Rice Ferment Filtrate`,
      HowtoUse: `Q : What UV Filters were used?
                    A : Ethylhexyl Triazone, Diethylamino Hydroxybenzoyl Hexyl Benzoate, Diethylhexyl Butamido Triazone, Methylene Bis-benzotriazolyl Tetramethylbutylphenol

                    Q : Do I need to use additional moisturizer together with this sunscreen?
                    A : For dry-combination skin, it is recommended to apply sunscreen after your serum or moisturizer.
                    For skin with excessive sebum or oily skin, you do not need to use additional moisturizer.

                    Q : How often should I reapply?
                    A : It is recommended to reapply every 2-3 hours.

                    Q : Can pregnant women use it?
                    A : Pregnant women can also use it, but during pregnancy, hormone changes are considerable and your skin can become very sensitive, so consult your doctor before use.

                    Q : Does it protect the skin from blue light?
                    A : It contains a filter that can even block blue light. However, please note that we did not conduct a separate clinical test for proving blue light block.`
    };
  },
};
</script>

<template>
    <div class="container">
        <img class="img" src="/src/assets/img/centella.png" alt="">

        <div class="small-img">
            <img src="/src/assets/img/centella.png" alt="">
            <img src="/src/assets/img/centella.png" alt="">
            <img src="/src/assets/img/centella.png" alt="">
            <img src="/src/assets/img/centella.png" alt="">
            <img src="/src/assets/img/centella.png" alt="">
            <img src="/src/assets/img/centella.png" alt="">
            <img src="/src/assets/img/centella.png" alt="">
        </div>
        <div class="listcome">Home / Toner / Centella Ampoule /</div>
        <div class="name">Centella Ampoule</div>
        <div class="rating-stars">
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star-half-stroke stars"></i>
                <span>1,936 Reviews</span>
        </div>
        <select class="opt1">
                <option>1</option>
                <option>2</option>
                <option>3</option>
                <option>4</option>
                <option>5</option>
                <option>6</option>
                <option>7</option>
                <option>8</option>
                <option>9</option>
                <option>10+</option>
        </select>
            <button class="cart">ADD TO CART</button>
            <button class="buy">BUY NOW</button>


            
            <div class="tabs">
            <div
                v-for="tab in tabs"
                :key="tab"
                :class="['tab', { active: activeTab === tab }]"
                @click="activeTab = tab"
            >
                {{ tab }}
            </div>
            </div>
            <div class="content">
                <p v-if="activeTab === 'Description'">Description content goes here.</p>
                <p v-if="activeTab === 'Ingredients'">{{ ingredients }}</p>
                <p v-if="activeTab === 'FAQ'">FAQ content goes here.</p>
                <p v-if="activeTab === 'How to Use'">{{ HowtoUse }}</p>
            </div>

        


            <div>
                <p class="detail">
                    See our detail product  
                </p>
                <div class="img1">
                    <img  src="/src/assets/img/Relief-Sun-1.webp" alt="">
                    <span class="title1">Suncare Never Felt So Hydrating</span>
                    <p class="text1">Experience Sun Care like never before with Beauty of Joseon's<br> Relief Sun. A lightweight, creamy organic sunscreen that provides<br> ultimate comfort while nourishing your skin.</p>
                </div>
            </div>

                <div class="img2">
                    <img  src="/src/assets/img/img2.webp" alt="">
                    <span class="title2">30% Rice Extract</span>
                    <p class="text2">Rice is a treasure trove of vitamins B, C, and E, amino acids, and minerals. This powerhouse<br> ingredient deeply moisturizes, leaving your skin replenished and glowing.</p>
                </div>

                <div class="img3">
                    <img  src="/src/assets/img/img3.webp" alt="">
                    <span class="title3">Grain Fermented Extracts</span>
                    <p class="text3">Enriched with vitamins, amino acids, and minerals, this harmonious blend nourishes your skin<br> with a wholesome dose of nutrition. They work synergistically to soothe, calm, and revitalize your <br>skin.</p>
                </div>
            
            <div class="vdo1">
                <video autoplay muted loop>
                    <source src="/src/assets/img/Mary&May Serum Collection.mp4">
                </video>

                    <span class="title4">Creamy Application, Swift Absorption</span>
                    <p class="text4">Experience the effortless glide of a light moisturizing cream<br> that seamlessly melds into your skin. No stickiness, no<br> waiting – just swift absorption, leaving behind a nourished,<br> radiant canvas</p>
            </div>


            <div class="imgrow1">
                <img src="/src/assets/img/toner1.webp" alt="">
            </div>
            <div class="imgrow2">
                <img src="/src/assets/img/toner2.jpg" alt="">
            </div>
            <div class="imgrow3">
                <img src="/src/assets/img/toner3.jpg" alt="">
            </div>

            <div class="textimgrow1">
                <span>Made From Nature</span>
                <p>
                  Our proprietary knit feels lightweight, breathable, and pleasantly cool thanks to a tree fiber material blend
                </p>
            </div>
            <div class="textimgrow2">
                <span>Wear-All-Day Support</span>
                <p>
                  Experience the comfort of SweetFoam®, our cushioned midsole made from sugarcane, providing all-day happiness for your feet
                </p>
            </div>
            <div class="textimgrow3">
                <span>100% Machine Washable</span>
                <p>
                  Our shoes are fully washable, making every step as clean as the first
                </p>
            </div>

            <div class="rating-starss">
  <p><span class="all-rate">4.5</span>
      <span class="fa fa-star checked star"></span>
      <span class="fa fa-star checked star"></span>
      <span class="fa fa-star checked star"></span>
      <span class="fa fa-star checked star"></span>
      <span class="fa fa-star-half checked star"></span>
         <span class="text-rate">paverage based on 5551 reviews.</span></p>

  <div class="row">
    <div class="side">
      <div> 
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
      </div>
    </div>
    <div class="middle">
      <div class="bar-container">
        <div class="bar-5"></div>
      </div>
    </div>
    <div class="side right">
      <div>3.9k</div>
    </div>
    <div class="side">
      <div>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
      </div>
    </div>
    <div class="middle">
      <div class="bar-container">
        <div class="bar-4"></div>
      </div>
    </div>
    <div class="side right">
      <div>1.4k</div>
    </div>
    <div class="side">
      <div>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
      </div>
    </div>
    <div class="middle">
      <div class="bar-container">
        <div class="bar-3"></div>
      </div>
    </div>
    <div class="side right">
      <div>170</div>
    </div>
    <div class="side">
      <div>
        <span class="fa fa-star checked star"></span>
        <span class="fa fa-star checked star"></span>
      </div>
    </div>
    <div class="middle">
      <div class="bar-container">
        <div class="bar-2"></div>
      </div>
    </div>
    <div class="side right">
      <div>69</div>
    </div>
    <div class="side">
      <div>
        <span class="fa fa-star checked star"></span>
      </div>
    </div>
    <div class="middle">
      <div class="bar-container">
        <div class="bar-1"></div>
      </div>
    </div>
    <div class="side right">
      <div>12</div>
    </div>
  </div>

  </div>

  <div ><span class="thanks">Thank you for</span>
    <p class="thanks2">When you tell someone they’re awesome, they’ll absolutely love it,<br> especially when they’ve spent time giving you feedback or signing up to your website.<br> Here’s how you can do that while saying a Thank You! </p>
  </div>


  <div class="moreproduct">
    View more products
  </div>
    <div><recommend2 /></div>

        <div class="icon">
            <a href=""><i class="fa-brands fa-facebook Facebook"></i></a>
            <a href=""><i class="fa-brands fa-tiktok Tiktok"></i></a>
            <a href=""><i class="fa-brands fa-youtube Youtube"></i></a>
            <a href=""><i class="fa-brands fa-instagram Instagram"></i></a>
        </div>

        <div><section class="footer">
        <div class="background">
            <div class="title">Follow Gladdy Smile Social Media</div>
        </div>
      <div class="footer-row">
        <div class="footer-col">
          <h4>Skin 1004</h4>
          <ul class="links">
            <li><a href="#">Mask</a></li>
            <li><a href="#">Toner</a></li>
            <li><a href="#">Cleanser</a></li>
            <li><a href="#">Sunscreen</a></li>
            <li><a href="#">Special Care</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h4>Beauty of Joseon</h4>
          <ul class="links">
            <li><a href="#">Serum</a></li>
            <li><a href="#">Cleanser</a></li>
            <li><a href="#">Sunscreen</a></li>
            <li><a href="#">Exfoliator</a></li>
            <li><a href="#">Moisturizer</a></li>
            <li><a href="#">Save with Sets</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h4>Mary & May</h4>
          <ul class="links">
            <li><a href="#">Serum</a></li>
            <li><a href="#">Cream</a></li>
            <li><a href="#">Sun Care</a></li>
            <li><a href="#">Toner/Lotion</a></li>
            <li><a href="#">Special Set</a></li>
            <li><a href="#">Miniature & Accessory</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h4>Cosrx</h4>
          <ul class="links">
            <li><a href="#">Minis</a></li>
            <li><a href="#">Treatments</a></li>
            <li><a href="#">Lip Care</a></li>
            <li><a href="#">Spot Patches</a></li>
            <li><a href="#">Sun Protection</a></li>
            <li><a href="#">Exfoliants & Scrubs</a></li>
          </ul>
        </div>
        
      </div>
    </section></div>
    </div>
</template>

<style scoped>
    *{
        padding: 0;
        margin: 0;
        box-sizing: border-box;
    }
    .container{
        width: 100%;
        height: 100%;
    }
    .img{
        width: 50%;
        height: auto;
        object-fit: cover;
        margin-left: 385px;
        margin-top: 150px;
    }
    .small-img{
        position: absolute;
        top: 133px;

    }
    .small-img img{
        width: 6%;
        height: auto;
        flex-direction: row;
        display: grid;
        margin-top: 17.5px;
        object-fit: cover;
        margin-left: 285px;
        cursor: pointer;
    }
    .name{
        position: absolute;
        font-size: 35px;
        font-weight: bold;
        margin-left: 1110px;
        top: 170px;
    }
    .listcome{
        position: absolute;
        font-size: 13px;
        margin-left: 1110px;
        top: 150px;
        cursor: pointer;
    }
    .rating-stars{
        position: absolute;
        font-size: 13px;
        margin-left: 1110px;
        top: 260px;
        cursor: pointer;
    }
    .rating-stars .stars{
        padding-inline: 5px;
    }
    .rating-stars span{
        font-size: 14px;
        font-weight: 500;
        padding-left: 5px;
    }
    .opt1{
        position: absolute;
        z-index: 99;
        padding-inline: 40px;
        padding-block: 10px;
        font-weight: 500;
        top: 330px;
        border-radius: 5px;
        margin-left: 70px;
    }
    .opt1:hover{
        border: 1px solid palevioletred;
    }
    .buy{
        position: absolute;
        top: 390px;
        margin-left: 69px;
        padding-inline: 240px;
        padding-block: 10px;
        font-weight: 500;
        background-image: linear-gradient(to right, pink , rgb(249, 83, 138));
        color: white;
        border: none;
        border-radius: 5px;
        z-index: 999;
    }
    .buy:hover{
        background-image: linear-gradient(to right, rgb(255, 152, 169) , rgb(245, 40, 108));
    }
    .cart{
        position: absolute;
        background: none;
        border: 1px solid black;
        margin-left: 220px;
        padding-block: 9.5px;
        padding-inline: 150px;
        font-weight: 500;
        border-radius: 5px;
        top: 330px;
    }
    .cart:hover{
        border: 1px solid palevioletred;
    }
    .description{
        position: absolute;
        top: 480px;
        margin-left: 1115px;
        cursor: pointer;
    }
    .description span:hover{
        color: palevioletred;
    }
    .ingredients{
        position: absolute;
        top: 480px;
        margin-left: 1300px;
        cursor: pointer;
    }
    .ingredients span:hover{
        color: palevioletred;
    }
    .howtouse{
        position: absolute;
        top: 480px;
        margin-left: 1480px;
        cursor: pointer;
    }
    .howtouse span:hover{
        color: palevioletred;
    }



    .tabs {
        position: absolute;
        display: flex;
        margin-bottom: 10px; /* Adjust spacing as needed */
        float: right;
        right: 310px;
        top: 460px;
    }

    .tab {
        padding: 10px;
        cursor: pointer;
        margin-right: 20px; /* Adjust spacing between tabs */
        font-weight: normal; /* Ensure font weight is consistent */
    }

    .tab.active {
        font-weight: bold;
        border-bottom: 2px solid pink; /* Highlight the active tab */
    }

    .tab:hover {
        border-bottom: 2px solid pink; /* Highlight the tab on hover */
    }

    .content {
        margin-top: 20px;
        position: absolute;
        width: 30%;
        right: 230px;
        top: 510px;
    }



    .detail{
        font-size: 30px;
        color: black;
        margin-left: 850px;
        margin-top: 200px;
    }
    
    .img1 img{
        margin-left: 950px;
        margin-top: 30px;
        margin-bottom: 20px;
    }
    .title1{
        position: absolute;
        color: black;
        font-size: 30px;
        font-weight: 500;
        margin-left: 350px;
        top: 1320px;
        z-index: 2;
        text-align: center;
    }
    .text1{
        position: absolute;
        font-size: 19px;
        color: black;
        margin-left: 300px;
        top: 1390px;
        text-align: center;
    }

    .img2 img{
        width: 700px;
        height: 650px;
        margin-left: 230px;
        margin-top: 30px;
        object-fit: cover;
    }
    .title2{
        position: absolute;
        color: black;
        font-size: 20px;
        margin-left: 520px;
        top: 2520px;
        z-index: 4;
        text-align: center; 
        left: 0;
    }
    .text2{
        position: absolute;
        color: black;
        font-size: 16px;
        margin-left: 260px;
        top: 2560px;
        z-index: 4;
        text-align: center; 
        left: 0;
    }
    .img3 img{
        width: 700px;
        height: 650px;
        margin-left: 972px;
        margin-top: -675px;
        object-fit: cover;
    }
    .title3{
        position: absolute;
        color: black;
        font-size: 20px;
        margin-left: 1200px;
        top: 2520px;
        z-index: 4;
        text-align: center; 
        left: 0;
    }
    .text3{
        position: absolute;
        color: black;
        font-size: 16px;
        margin-left: 980px;
        top: 2560px;
        z-index: 4;
        text-align: center; 
        left: 0;
    }

    .vdo1 video{
        position: absolute;
        height: auto;
        width: 720px;
        margin-top: 150px;
        left: 0;
        margin-left: 230px;
    }
    .title4{
        position: absolute;
        color: black;
        font-size: 25px;
        margin-left: 1120px;
        font-weight: 500;
        top: 2790px;
        z-index: 4;
        text-align: center; 
        left: 0;
    }
    .text4{
        position: absolute;
        color: black;
        font-size: 16px;
        margin-left: 1120px;
        top: 2840px;
        z-index: 4;
        text-align: center; 
        left: 0;
        text-align: left;
    }
   


    /* rating star */
    .container .rating-starss{
        margin-top: 200px;
        margin-left: 200px;
        float: left;
        width: 800px;
    }

.heading {
  font-size: 25px;
  margin-right: 10px;

}

.fa {
  font-size: 25px;
}

.checked {
  color: rgba(255, 171, 16, 0.798);
  top: 30px;
  padding-bottom: 8px;
}

/* Three column layout */
.side {
  float: left;
  width: 15%;
  margin-top:10px;
}

.middle {
  margin-top:10px;
  float: left;
  width: 70%;
}

/* Place text to the right */
.right {
  font-size: 14px;
  font-weight: 600;
    padding-left: 10px;
}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* The bar container */
.bar-container {
  width: 100%;
  background-color: #cfcece;
  text-align: center;
  color: white;
}
.star{
  font-size: 15px;
}
.all-rate{
  font-size: 20px;
  font-weight: 800;
  padding-right: 10px;
}
.text-rate{
  font-size: 16px;
  padding-left: 5px;
}

/* Individual bars */
.bar-5 {width: 89%; height: 6px;border-radius: 10px; margin-top: 9px; margin-left: -15px; background-color: palevioletred;}
.bar-4 {width: 30%; height: 6px;border-radius: 10px; margin-top: 9px; margin-left: -15px; background-color: palevioletred;}
.bar-3 {width: 10%; height: 6px;border-radius: 10px; margin-top: 9px; margin-left: -15px; background-color: palevioletred;}
.bar-2 {width: 5%; height: 6px;border-radius: 10px; margin-top: 9px; margin-left: -15px; background-color: palevioletred;}
.bar-1 {width: 3%; height: 6px;border-radius: 10px; margin-top: 9px; margin-left: -15px; background-color: palevioletred;}


.thanks{
    position: absolute;
    font-size: 30px;
    margin-top: 240px;
    margin-left: 300px;
    font-weight: 500;
}
.thanks2{
    position: absolute;
    font-size: 18px;
    color: black;
    margin-top: 320px;
    margin-left: 1050px;
    text-align: center;
}

.imgrow1 img{
    margin-top: 733px;
    height: 540px;
    width: 400px;
    object-fit: cover;
    margin-left: 340px;
}
.imgrow2 img{
    margin-top: -570px;
    height: 540px;
    width: 400px;
    object-fit: cover;
    margin-left: 750px;
}
.imgrow3 img{
    margin-top: -619px;
    height: 540px;
    width: 400px;
    object-fit: cover;
    margin-left: 1160px;
}
.textimgrow1 span{
  position: absolute;
    font-size: 28px;
    font-weight: bold;
    margin-left: 340px;
    top: 3815px;
}
.textimgrow1 p{
    font-size: 17px;
    margin-left: 340px;
    margin-top: -30px;
    width: 400px;
    margin-top: 15px;
    font-weight: 400;
}
.textimgrow2 span{
    position: absolute;
    font-size: 28px;
    font-weight: bold;
    margin-left: 753px;
    top: 3815px;
}
.textimgrow2 p{
    font-size: 17px;
    margin-left: 750px;
    width: 400px;
    margin-top: -80px;
    font-weight: 400;
}
.textimgrow3 span{
    position: absolute;
    font-size: 28px;
    font-weight: bold;
    margin-left: 1159px;
    top: 3815px;
}
.textimgrow3 p{
    font-size: 17px;
    margin-left: 1165px;
    width: 400px;
    margin-top: -80px;
    font-weight: 400;
}
.footer {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, 50%);
  width: 100%;
  background: black;
  margin-top: 4650px;
}
.background{
    width: 100%;
    height: 250px;
    background-color: whitesmoke;
    border: none;
    outline: none;
}
.title{
    font-family: "Zain", sans-serif;
    font-weight: 400;
    font-style: normal;
    font-size: 40px;
    color: black;
    margin-left: 650px;
    padding-top: 30px;
    bottom: 0;
}

.footer .footer-row {
  display: flex;
  width: 100%;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 3.5rem;
  padding: 60px;
  
}

.footer-row .footer-col h4 {
  color: #fff;
  font-size: 1.2rem;
  font-weight: 400;
}

.footer-col .links {
  margin-top: 20px;
}

.footer-col .links li {
  list-style: none;
  margin-bottom: 10px;
}

.footer-col .links li a {
  text-decoration: none;
  color: #bfbfbf;
}

.footer-col .links li a:hover {
  color: #fff;
}
.moreproduct{
    font-size: 35px;
    font-weight: bold;
    float: left;
    margin-top: 150px;
    margin-left: 100px;
}
.icon{
    position: absolute;
    font-size: 50px;
    margin-left: 700px;
    margin-top: 320px;
    z-index: 44;
}
.Facebook{
    padding-right: 100px;
    color: black;
}
.Tiktok{
    padding-right: 100px;
    color: black;
}
.Youtube{
    padding-right: 100px;
    color: black;
}
.Instagram{
    padding-right: 100px;
    color: black;
}
</style>