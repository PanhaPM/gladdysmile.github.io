<script setup>
    import ListShop from "./ListShop.vue"

    let lastScrollTop = 0;
  
    window.onscroll = function() {
      scrollFunction();
    };
  
    function scrollFunction() {
      let st = window.pageYOffset || document.documentElement.scrollTop;
  
      if (st > lastScrollTop) {
        // Downscroll
        if (document.body.scrollTop > 80 || document.documentElement.scrollTop > 80) {
        document.getElementById("navbar").style.padding = "5px 10px";
        document.getElementById("navbar").style.top = "-75px";
        document.getElementById("navbar").style.transition = "0.9s";
        document.getElementById("logo").style.display = "block";


        }
      } else {
        // Upscroll
        document.getElementById("navbar").style.padding = "5px 10px";
        document.getElementById("logo").style.display = "block";
        document.getElementById("navbar").style.transition = "0.9s";
        document.getElementById("navbar").style.top = "0px";
      }
  
      lastScrollTop = st <= 0 ? 0 : st; // For Mobile or negative scrolling
    }
  </script>
  

<template>
    <div>
      <div id="navbar">
        <a href="#default" id="logo">GS</a>
  
        <nav class="menu">
          <ul>
            <li><a href="#">New in</a></li>
            <li><a href="#">Shop All</a></li>
            <li><a href="#">Toner</a></li>
            <li><a href="#">Serum</a></li>
            <li><a href="#">Cleansers</a></li>
            <li><a href="#">Lip Care</a></li>
            <li><a href="#">Masks</a></li>
            <li><a href="#">Moisturizers</a></li>
            <li><a href="#">Treatments</a></li>
          </ul>
          <div class="login-icon">
            <a><i class="fa-solid fa-user user"></i></a>
            <a><i class="fa-solid fa-heart heart"></i></a>
            <a><i class="fa-solid fa-location-dot location"></i></a>
            <a><i class="fa-solid fa-dollar-sign usd"></i></a>
            <a><i class="fa-solid fa-bars menu"></i></a>
        </div>
        </nav>
      </div>
  
      <div>
        <ListShop />
      </div>
    </div>
  </template>
  
  <style scoped>
    * {
      box-sizing: border-box;
    }
  
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
    }
  
    #navbar {
      overflow: hidden;
      background-color: black;
      padding: 10px 10px;
      transition: 0.4s;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 99;
    }
  
    #navbar a {
      float: left;
      color: black;
      text-align: center;
      padding: 12px;
      text-decoration: none;
      font-size: 18px;
      line-height: 25px;
      outline: none;
    }
  
    #navbar #logo {
      font-family: "Playwrite CU", cursive;
      font-optical-sizing: auto;
      font-weight: bold;
      font-style: normal;
      position: absolute;
      text-align: center;
      left: 50%;
      transform: translateX(-50%);
      font-size: 20px;
      color: palevioletred;
      text-decoration: none;
      width: 100%;
      background-color: black;
      padding-bottom: 27px;
      padding-top: 30px;
      transition: 0.9s;
      border-radius: none;
      top: 0px;
      
    }
  
    #navbar nav {
      width: 100%;
    }
  
    #navbar .menu {
      display: flex;
      justify-content: center;
      padding-top: 70px;
    }
  
    #navbar ul {
      list-style: none;
      padding: 0;
      margin: 0;
      display: flex;
    }
  
    #navbar ul li {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
  
    #navbar ul li a {
      color: white;
      font-size: 20px;
      text-decoration: none;
      padding: 10px 30px;
      text-align: center;
      font-weight: 500;
    }
  
    @media screen and (max-width: 580px) {
      #navbar {
        padding: 10px 10px !important;
      }
  
      #navbar a {
        float: none;
        display: block;
        text-align: left;
      }
    }

    .login-icon{
        position: absolute;
        font-size: 20px;
        top: 18px;
        right: 40px;
        cursor: pointer;
        display: flex;
        justify-content: space-between;
        color: white;
        z-index: 100;
    }
    .login-icon a .user {
        color: white;
        margin-left: 60px;
    }
    .login-icon a .heart{
        color: white;
        margin-left: 60px;
    }
    .login-icon a .location{
        color: white;
        margin-left: 60px;
    }
    .login-icon a .usd{
        color: white;
        margin-left: 60px;
        font-weight: bold;
    }
    .login-icon a .menu{
        color: white;
        margin-left: 60px;
        font-weight: bold;
        margin-top: -65px;
    }




  </style>
  
  