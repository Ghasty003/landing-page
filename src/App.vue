<template>
  <main class="parent">
    <NavBar />

    <img src="./assets/Abstract.png" alt="image">

    <div class="header_container">

      <div class="btn_con">
        <h2>Tell a better brand story</h2>
        <p>Warrant present garrets limited cordial in inquiry to. Supported me sweetness behaviour shameless excellent so arranging.</p>

        <div>
          <button>Get Started</button>
          <button>Contact Us</button>
        </div>
      </div>

      <div>

        <div class="profile-con">

          <div class="profile">
            <img src="./assets/profile.png" alt="profile">

            <div>
              <h3>Amanda M. Data</h3>
              
              <span>
                <p>Your Growth</p>
                <h4>3,000</h4>
              </span>
            </div>
          </div>

          <img src="./assets/Card10.png" alt="image">

        </div>

      </div>

      <div class="media_parent">

        <div>
          <div>
            <p>Media Type</p>
            <img src="./assets/download.png" alt="image">
          </div>

          <img src="./assets/media.png" alt="image">
        </div>

        <div>
          <p>14k</p>
          <div>
            <p>Follower Growth</p>

            <div>
              <img src="./assets/Rectangle1.png" alt="image">
              <br />
              <img src="./assets/Rectangle2.png" alt="image">
            </div>
          </div>
        </div>

        <div>
          <img src="./assets/Group.png" alt="image">
          <img src="./assets/Group2.png" alt="image">
          <img src="./assets/Group1.png" alt="image">
        </div>

      </div>
    </div>

  </main>

  <div class="bg_irr">
    <img src="./assets/irregular.png" alt="image">
  </div>

  <header>

    <div>
      <img src="./assets/logo1.png" alt="logo">
      <img src="./assets/logo2.png" alt="logo">
      <img src="./assets/logo3.png" alt="logo">
      <img src="./assets/logo4.png" alt="logo">
      <img src="./assets/logo1.png" alt="logo">
    </div>

    <div>
      <h2>What we Offer?</h2>
      <p> in virtual space through communication platforms. Durable relations that extend beyond immediate genealogical ties.</p>
    </div>


    <div>
      <HeaderCard :img="img1" />
      <HeaderCard :img="img1" />
      <HeaderCard :img="img1" />
      <HeaderCard :img="img1" />
      <HeaderCard :img="img1" />
      <HeaderCard :img="img1" />
    </div>

  </header>


  <section class="sec_1">
    <div>
      <h3>How it Works?</h3>
      <p>Resolving neglected sir tolerably but existence conveying for. Day his put off unaffected literature partiality inhabiting.</p>

      <img src="./assets/Card1.png" alt="image">
    </div>

    <div>
      <img src="./assets/Card2.png" alt="image">
      <img src="./assets/Card3.png" alt="image">

      <img src="./assets/irregular2.png" alt="image">
    </div>
  </section>

  <div class="arrow_up">
    <img src="./assets/Abstract2.png" alt="image">
  </div>

  <section class="product_header">
    <div>
      <h3>Our plans scale with your product</h3>
      <p>in virtual space through communication platforms.</p>
    </div>

    <div>
      <img src="./assets/product-card.png" alt="image">
      <img src="./assets/product-card2.png" alt="image">
      <img src="./assets/product-card3.png" alt="image">
    </div>
  </section>

  <section class="reviews">
    <div>
      <h3>What Our Clients Say About Us</h3>
      <p>Community development is often linked with community work or community planning, and may involve stakeholders, foundations.</p>
    </div>

    <div>

    </div>
  </section>

</template>

<script setup lang="ts">
import NavBar from "./components/NavBar.vue";
import HeaderCard from "@/components/HeaderCard.vue";


const img1 = new URL("./assets/header1.png", import.meta.url);


</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  background-color:white;
}

main {
  background-image: url("./assets/Lines.png");
  background-position: center;
  background-repeat: no-repeat;
  // background-size: contain;
}


.bg_irr {
  width: 100%;
  position: absolute;
  z-index: -100;
  top: 270px;

  img {
    width: 100%;
  }
}

.header_container {
  display: flex;
  justify-content: space-around;
  align-items: center;
  position: relative;
  padding-left: 100px;
  transform: translateY(-70px);
}

.btn_con {
  // background: #000;
  width: 500px;
  
  h2 {
    font-size: 85px;
    background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), #3E4581;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    line-height: 88px;
  }

  p {
    font-size: 20px;
    color: #3E4581;
    margin: 40px 0;
  }


  button {
    width: 180px;
    height: 48px;
    

    &:first-child {
      background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), linear-gradient(106.23deg, #4EF0F0 0%, #05C580 100%);
      border-radius: 5px;
      border: none;
      color: white;
    }

    &:last-child {
      background: transparent;
      border-radius: 5px;
      border: 2px solid #AE67FA;
      background: linear-gradient(106.23deg, #AE68FA 0%, #F1966E 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      margin-left: 20px;
    }
  }
}

.profile-con {
  // background-color: red;
  position: relative;
  width: 350px;

  > img {
    transform: translate(-20px, 250px);
  }
}


.profile {
  width: 188px;
  height: 217.89px;
  background: #FFFFFF;
  box-shadow: 0px 56px 63px rgba(0, 0, 0, 0.22);
  border-radius: 10px;
  position: absolute;
  right: 0;



  img {
    position: absolute;
    top: -35px;
    right: -35px;
  }


  div {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    position: relative;
    height: 100%;

    span {
      position: absolute;
      bottom: 20px;
    }

    h3 {
      width: 127px;
      font-size: 20px;
      text-align: center;
      color: #3E4581;
      opacity: 0.96;
      position: absolute;
      top: 30px;
    }

    h4 {
      font-weight: 700;
      font-size: 30px;
      text-align: center;
      width: 90px;
      background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), linear-gradient(106.23deg, #4EF0F0 0%, #05C580 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    p {
      width: 84px;
      font-size: 14px;
      text-align: center;
      color: #3E4581;
    }
  }
}


.media_parent {
  // background: orange;
  width: 320px;


  > div:first-child {
    background: #FFFFFF;
    box-shadow: 0px 56px 63px rgba(0, 0, 0, 0.22);
    border-radius: 10px;
    width: 300px;
    position: relative;
    left: 50%;
    transform: translateX(-50%);
    padding-top: 30px;

    > div {
      display: flex;
      align-items: center;
      justify-content: space-around;
    }
  }

  > div:nth-child(2) {
    width: 100%;
    height: 112.94px;
    background: #FFFFFF;
    box-shadow: 0px 56px 63px rgba(0, 0, 0, 0.22);
    border-radius: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;


    > p {
      background: #EADFFB;
      width: fit-content;
      padding: 5px;
      border-radius: 6px;
      font-weight: 600;
      font-size: 40px;
      color: #3E4581;
      text-align: center;
    }
  }

  > div:nth-child(3) {
    background: #FFFFFF;
    box-shadow: 0px 56px 63px rgba(0, 0, 0, 0.22);
    border-radius: 10px;
    margin-top: 20px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 200px;
    height: 50px;
    position: relative;
    left: 50%;
    transform: translateX(-50%);
  }
}


header {
  margin-top: 150px;

  > div:first-child {
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 0 10px;
  }

  > div:nth-child(2) {
    margin-top: 150px;
    
    h2 {
      text-align: center;
      background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), #3E4581;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      font-size: 60px;
    }

    p {
      font-size: 20px;
      text-align: center;
      color: #3E4581;
      width: 600px;
      position: relative;
      left: 50%;
      transform: translateX(-50%);
      margin-top: 20px;
    }
  }

  > div:nth-child(3) {
    margin-top: 70px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;
    padding: 0 180px;
    gap: 20px;
  }
}

.sec_1 {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  margin-top: 150px;
  position: relative;

  > div:first-child, > div:nth-child(2) {
    position: relative;
    z-index: 100;

    img {
      width: 100%;
      text-align: start;
    }
  }

  > div:first-child {
    width: 420px;

    h3 {
      text-align: center;
      font-size: 60px;
      background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), #3E4581;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    p {
      font-style: normal;
      font-weight: 500;
      color: #3E4581;
      margin: 30px 0;
    }
  }

  > div:nth-child(2) {
    position: relative;
    width: 400px;
    text-align: start;

    img:nth-child(3) {
      // display: none;
      position: absolute;
      left: 132px;
      z-index: -100;
      top: 200px;
      // background: #000;
      // width: 300px;
    }
  }
}

.arrow_up {
  position: relative;
  top: -100px;
}

.product_header {
  margin-top: -120px;
  
  > div:first-child {

    h3 {
      text-align: center;
      background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), #3E4581;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      font-size: 60px;
      width: 720px;
      margin: auto;
    }

    p {
      text-align: center;
      color: #3E4581;
      font-size: 20px;
      margin-top: 20px;
    }
  }

  > div:last-child {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 0 20px;
    margin-top: 80px;

    img {
      width: 300px;
    }
  }
}

.reviews {
  margin-top: 150px;

  > div:first-child {
    
    h3 {
      text-align: center;
      background: linear-gradient(89.97deg, #AE67FA 1.84%, #F49867 102.67%), #3E4581;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      font-size: 60px;
      width: 720px;
      margin: auto;
    }

    p {
      text-align: center;
      color: #3E4581;
      font-size: 20px;
      margin-top: 20px;
      width: 600px;
      margin: {
        left: auto;
        right: auto;
      }
    }
  }
}

</style>
