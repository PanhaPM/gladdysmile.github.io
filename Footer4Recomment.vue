<template>
    <section class="footer">
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
    </section>
</template>

<style scoped>
    /* Importing Google font - Open Sans */
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;500;600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Open Sans', sans-serif;
}

.footer {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, 50%);
  width: 100%;
  background: black;
  margin-top: 1900px;
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

</style>