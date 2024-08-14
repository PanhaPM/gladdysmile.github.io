<template>
    <div class="container">

        <div class="box">
            <div class="box1">
                <img src="/src/assets/img/mountain.jpg" alt="">
                <p class="brand1">Mary and May</p>
                <p class="name1">Try Mary & May Hyaluronic Acid Solution</p>
                <p class="pover1">
                    Mary & May is a genuine clean beauty
                    <br> skincare brand. It is our mission to provide 
                    <br> consumers with highly effective skincare
                    <br> products, packed with active ingredients
                    <br> that are good
                </p>
                <button>Explore Here</button>
            </div>
        </div>


        <div class="box">
            <div class="box2">
                <img src="/src/assets/img/mountain.jpg" alt="">
                <p class="brand2">Mary and May</p>
                <p class="name2">Try Mary & May Hyaluronic Acid Solution</p>
                <p class="pover2">
                    Mary & May is a genuine clean beauty
                    <br> skincare brand. It is our mission to provide 
                    <br> consumers with highly effective skincare
                    <br> products, packed with active ingredients
                    <br> that are good
                </p>
                <button>Explore Here</button>
            </div>
        </div>


        <div class="box">
            <div class="box3">
                <img src="/src/assets/img/mountain.jpg" alt="">
                <p class="brand3">Mary and May</p>
                <p class="name3">Try Mary & May Hyaluronic Acid Solution</p>
                <p class="pover3">
                    Mary & May is a genuine clean beauty
                    <br> skincare brand. It is our mission to provide 
                    <br> consumers with highly effective skincare
                    <br> products, packed with active ingredients
                    <br> that are good
                </p>
                <button>Explore Here</button>
            </div>
        </div>


        <div class="box">
            <div class="box4">
                <img src="/src/assets/img/mountain.jpg" alt="">
                <p class="brand4">Mary and May</p>
                <p class="name4">Try Mary & May Hyaluronic Acid Solution</p>
                <p class="pover4">
                    Mary & May is a genuine clean beauty
                    <br> skincare brand. It is our mission to provide 
                    <br> consumers with highly effective skincare
                    <br> products, packed with active ingredients
                    <br> that are good
                </p>
                <button>Explore Here</button>
            </div>
        </div>

        
    </div>
</template>

<style scoped>
    *{
        padding: 0;
        margin: 0;
        box-sizing: border-box;
    }
    .container{
        padding: 0;
    }

    .box {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: space-between;
        cursor: pointer;
    }

    .box1 {
        width: 370px;
        height: 500px;
        background-color: #F5F5F5;
        margin: 80px auto;
        border-radius: 10px;
        white-space: nowrap;
        transition: 0.5s;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        position: relative;
        cursor: pointer;
        margin-top: 100px;
        margin-left: 100px;
    }

    .box1 img {
        width: 370px;
        height: 150px;
        object-fit: cover;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
        transition: 0.3s;
    }

    .box1 .brand1,
    .box1 .name1,
    .box1 .pover1 {
        margin: 20px 30px;
        transition: 0.3s;
    }

    .box1 .brand1 {
        font-size: 22px;
        color: gray;
        font-weight: 500;
    }

    .box1 .name1 {
        font-size: 14px;
        color: gray;
        font-weight: bold;
    }

    .box1 .pover1 {
        font-size: 16px;
        color: black;
        font-weight: 500;
        display: none;
    }

    .box1 button {
        border: none;
        background-color: white;
        font-size: 15px;
        border-radius: 30px;
        padding: 10px;
        font-weight: bold;
        color: black;
        position: absolute;
        bottom: 30px;
        left: 30px;
        transition: 0.3s;
    }

    .box1:hover {
        transform: scale(1.02);
        z-index: 5;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .box1:hover img {
        opacity: 0;
        display: none;
    }

    .box1:hover .pover1 {
        display: block;
    }

    .box1:hover .brand1,
    .box1:hover .name1 {
        margin-top: 10px;
        opacity: 1;
        transition: margin-top 1s, opacity 1;
    }

    .box1:hover .pover1 {
        opacity: 1;
        transition: opacity 1s;
    }

    .box1:hover button{
        background-color: black;
        color: white;
    }


    .box {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: space-between;
        cursor: pointer;
    }

    .box2 {
        width: 370px;
        height: 500px;
        background-color: #F5F5F5;
        margin: 80px auto;
        border-radius: 10px;
        white-space: nowrap;
        transition: 0.5s;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        position: relative;
        cursor: pointer;
        margin-top: -580px;
        margin-left: 550px;
    }

    .box2 img {
        width: 370px;
        height: 150px;
        object-fit: cover;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
        transition: 0.3s;
    }

    .box2 .brand2,
    .box2 .name2,
    .box2 .pover2 {
        margin: 20px 30px;
        transition: 0.3s;
    }

    .box2 .brand2 {
        font-size: 22px;
        color: gray;
        font-weight: 500;
    }

    .box2 .name2 {
        font-size: 14px;
        color: gray;
        font-weight: bold;
    }

    .box2 .pover2 {
        font-size: 16px;
        color: black;
        font-weight: 500;
        display: none;
    }

    .box2 button {
        border: none;
        background-color: white;
        font-size: 15px;
        border-radius: 30px;
        padding: 10px;
        font-weight: bold;
        color: black;
        position: absolute;
        bottom: 30px;
        left: 30px;
        transition: 0.3s;
    }

    .box2:hover {
        transform: scale(1.02);
        z-index: 5;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .box2:hover img {
        opacity: 0;
        display: none;
    }

    .box2:hover .pover2 {
        display: none;
    }

    .box2:hover .brand2,
    .box2:hover .name2 {
        margin-top: 10px;
        opacity: 1;
        transition: margin-top 1s, opacity 1;
    }

    .box2:hover .pover2 {
        opacity: 1;
        transition: opacity 1s;
        display: block;
    }

    .box2:hover button{
        background-color: black;
        color: white;
    }


    .box {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: space-between;
        cursor: pointer;
    }

    .box3 {
        position: absolute;
        width: 370px;
        height: 500px;
        background-color: #F5F5F5;
        margin: 80px auto;
        border-radius: 10px;
        white-space: nowrap;
        transition: 0.5s;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        position: relative;
        cursor: pointer;
        margin-top: -580px;
        margin-left: 1000px;
    }

    .box3 img {
        width: 370px;
        height: 150px;
        object-fit: cover;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
        transition: 0.3s;
    }

    .box3 .brand3,
    .box3 .name3,
    .box3 .pover3 {
        margin: 20px 30px;
        transition: 0.3s;
    }

    .box3 .brand3 {
        font-size: 22px;
        color: gray;
        font-weight: 500;
    }

    .box3 .name3 {
        font-size: 14px;
        color: gray;
        font-weight: bold;
    }

    .box3 .pover3 {
        font-size: 16px;
        color: black;
        font-weight: 500;
        display: none;
    }

    .box3 button {
        border: none;
        background-color: white;
        font-size: 15px;
        border-radius: 30px;
        padding: 10px;
        font-weight: bold;
        color: black;
        position: absolute;
        bottom: 30px;
        left: 30px;
        transition: 0.3s;
    }

    .box3:hover {
        transform: scale(1.02);
        z-index: 5;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .box3:hover img {
        opacity: 0;
        display: none;
    }

    .box3:hover .pover3 {
        display: block;
    }

    .box3:hover .brand3,
    .box3:hover .name3 {
        margin-top: 10px;
        opacity: 1;
        transition: margin-top 1s, opacity 1;
    }

    .box3:hover .pover3 {
        opacity: 1;
        transition: opacity 1s;
    }

    .box3:hover button{
        background-color: black;
        color: white;
    }


    .box {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: space-between;
        cursor: pointer;
    }

    .box4 {
        position: absolute;
        width: 370px;
        height: 500px;
        background-color: #F5F5F5;
        margin: 80px auto;
        border-radius: 10px;
        white-space: nowrap;
        transition: 0.5s;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        position: relative;
        cursor: pointer;
        margin-top: -580px;
        margin-left: 1450px;
    }

    .box4 img {
        width: 370px;
        height: 150px;
        object-fit: cover;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
        transition: 0.3s;
    }

    .box4 .brand4,
    .box4 .name4,
    .box4 .pover4 {
        margin: 20px 30px;
        transition: 0.3s;
    }

    .box4 .brand4 {
        font-size: 22px;
        color: gray;
        font-weight: 500;
    }

    .box4 .name4 {
        font-size: 14px;
        color: gray;
        font-weight: bold;
    }

    .box4 .pover4 {
        font-size: 16px;
        color: black;
        font-weight: 500;
        display: none;
    }

    .box4 button {
        border: none;
        background-color: white;
        font-size: 15px;
        border-radius: 30px;
        padding: 10px;
        font-weight: bold;
        color: black;
        position: absolute;
        bottom: 30px;
        left: 30px;
        transition: 0.3s;
    }

    .box4:hover {
        transform: scale(1.02);
        z-index: 5;
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .box4:hover img {
        opacity: 0;
        display: none;
    }

    .box4:hover .pover4 {
        display: block;
    }

    .box4:hover .brand4,
    .box4:hover .name4 {
        margin-top: 10px;
        opacity: 1;
        transition: margin-top 1s, opacity 1;
    }

    .box4:hover .pover4 {
        opacity: 1;
        transition: opacity 1s;
    }

    .box4:hover button{
        background-color: black;
        color: white;
    }



</style>