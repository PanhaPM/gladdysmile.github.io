<script setup>
    import { ref } from 'vue'
    const itemList = ref(
        [
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
            {
                title: "Dynasty Cream",
                text1: "Top",
                price1: "From $15.00",
                price2: "$9.99",
                img:  "/src/assets/img/b4.png",
                img1: "/src/assets/img/b4.png",
                img2: "/src/assets/img/b 2.png"
            },
        ]
    )

    const Newimg = (data) => {
        console.log(data)
        data.img = data.img2

    }
    const Oldimg = (data) => {
        console.log(data)
        data.img = data.img1
    }

</script>

<template>
    <div class="body">
      <div class="container">
        <div class="product" v-for="(data, i) in itemList" :key="i" >
          <p class="top">{{ data.text1 }}</p>

          <div class="img" @mouseover="Newimg(data)" @mouseleave="Oldimg(data)">
             <img :src="data.img">
          </div>
          
          
          <p>{{ data.title }}</p>
          <p class="reviews">
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star stars"></i>
                <i class="fa-solid fa-star-half-stroke stars"></i>
                540 Reviews</p>
          <p class="original-price">{{ data.price1 }}</p><span class="price">{{ data.price2 }}</span>
        </div>
                
      </div>
    </div>
  </template>
  

  <style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  
}

body {
  font-family: Arial, sans-serif;
  display: flex;
  justify-content: center;
}

.container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 30px;
  width: 100%;
  margin-left: 440px;
  margin-top: 200px;
}

.product {
  text-align: center;
  width: 100%; /* Ensure it takes full column width */
}

.product img {
  width: 335px;
  height: 335px;
  cursor: pointer;
}

.reviews {
    top: 4px;
    color: #888;
}
.original-price {
    color: #888;
    text-decoration: line-through;
}

.price {
  font-weight: bold;
}
.stars{
    color: #FFA41C;
    font-size: 14px;   
}
.top{
    position: absolute;
    padding-block: 3px;
    padding-inline: 15px;
    margin: 7px;
    z-index: 2;
    color: white;
    font-size: 15px;
    background-color: rgba(216, 112, 147, 0.799);
}
</style>


