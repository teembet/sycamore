<template>
  <div class="home">
    <v-carousel hide-delimiters height="470">
      <v-carousel-item v-for="(item, i) in items" :key="i" :src="item.src">
        <div class="slider">
          <div class="text-content">
            <h1 style="width:470px;font-size:37px">
              You deserve the very best!
            </h1>
            <p style="font-size:14px;">
              You can get it just now, then pay later
            </p>
          </div>
        </div>
      </v-carousel-item>
    </v-carousel>
    <br />
    <v-row>
      <v-col cols="6" md="3">
        <v-card class="option-card">
          <v-row style="padding: 0 20px 0 20px">
            <v-col cols="3">
              <img
                style="margin-top:0"
                height="40"
                src="../assets/option1.png"
                alt=""
              />
            </v-col>
            <v-col cols="9" style="line-height:40px;font-weight:bold">
              Select product
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="6" md="3">
        <v-card class="option-card">
          <v-row style="padding: 0 20px 0 20px">
            <v-col cols="3">
              <img
                style="margin-top:0"
                height="40"
                src="../assets/option2.png"
                alt=""
              />
            </v-col>
            <v-col cols="9" style="line-height:40px;font-weight:bold">
              Upload product
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="6" md="3">
        <v-card class="option-card">
          <v-row style="padding: 0 20px 0 20px">
            <v-col cols="3">
              <img
                style="margin-top:0"
                height="40"
                src="../assets/option3.png"
                alt=""
              />
            </v-col>
            <v-col cols="9" style="line-height:40px;font-weight:bold">
              Pay 30% Upfront
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="6" md="3">
        <v-card class="option-card">
          <v-row style="padding: 0 20px 0 20px">
            <v-col cols="3">
              <img
                style="margin-top:0"
                height="40"
                src="../assets/option4.png"
                alt=""
              />
            </v-col>
            <v-col cols="9" style="line-height:40px;font-weight:bold">
              Get delivery in 2 days
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
    <br />
    <div style="text-align:center;margin-top:20px;margin-bottom:20px;">
      <h2 class="section-header">Product Category</h2>
    </div>
    <div style="padding:20px">
      <v-row>
        <v-col
          cols="6"
          v-for="item in category"
          :key="item"
          style="padding:30px 20px 0 20px"
        >
          <v-card
            :color="item.color"
            flat
            style="height:280px;border-radius:15px"
          >
            <v-row style="padding: 0 20px 0 20px">
              <v-col cols="6" style="padding-top:70px; padding-left:30px">
                <h2 style="font-size:30px;color:white">{{ item.title }}</h2>
                <br />
                <v-btn
                  outlined
                  color="white"
                  depressed
                  style="text-transform:none;"
                  dark
                  >Buy Now
                  <v-icon style="margin-left:10px;font-size:20px" dark
                    >mdi-arrow-right</v-icon
                  ></v-btn
                >
              </v-col>
              <v-col cols="6" style="line-height:40px;font-weight:bold">
                <img :src="item.img" alt="" />
              </v-col>
            </v-row>
          </v-card>
        </v-col>
        <v-col cols="6" style="padding:30px 20px 0 20px">
          <v-card color="#EEF0FF" flat style="height:280px;border-radius:15px">
            <v-row style="padding: 0 20px 0 20px">
              <v-col cols="6" style="padding-top:70px;padding-left:30px">
                <h2 style="font-size:30px;color:black">Air Conditioner</h2>
                <br />
                <v-btn
                  outlined
                  color="black"
                  depressed
                  style="text-transform:none;"
                  >Buy Now
                  <v-icon style="margin-left:10px;font-size:20px" dark
                    >mdi-arrow-right</v-icon
                  ></v-btn
                >
              </v-col>
              <v-col
                cols="6"
                style="text-align:center;line-height:40px;font-weight:bold"
              >
                <img src="../assets/ac.png" alt="" />
              </v-col>
            </v-row>
          </v-card>
        </v-col>
      </v-row>
      <br /><br /><br />
      <div style="text-align:center">
        <v-btn
          x-large
          style="font-weight:bold;text-transform:none;"
          outlined
          color="black"
          >See all Products</v-btn
        >
      </div>
    </div>

    <div class="botttom-banner">
      <h2 style="font-size:30px;color:#E23939">How it works</h2>
      <br />
      <div style="width:600px">
        <li>Available to Lagos Residents only</li>
        <li>Available to salaried workers</li>
        <li>
          30% upfront payment must be received before items are delivered. 70%
          balance to be paid up on your next salary pay day
        </li>
        <li>
          Applicable interest rate as indicated is indicated on each basket.
        </li>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",

  data() {
    return {
      items: [
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],
      category: [
        {
          color: "#BD1E4A",
          title: "Phones, Tablet and Laptop",
          img: require("../assets/lappy.png"),
        },
        {
          color: "#1B1333",
          title: "Television Set",
          img: require("../assets/tv.png"),
        },
        {
          color: "#747C98",
          title: "Refrigerators and Freezers",
          img: require("../assets/fridgee.png"),
        },
        {
          color: "#303030",
          title: "Gas Cookers",
          img: require("../assets/oven.png"),
        },
        {
          color: "#532010",
          title: "Generators",
          img: require("../assets/gen.png"),
        },
      ],
    };
  },
};
</script>

<style>
.botttom-banner {
  margin-top: 50px;
  overflow: hidden;
  border-radius: 15px;
  padding: 50px 80px 50px 80px;
  background-image: url("../assets/Nav.png");
  background-size: cover;
}
.section-header {
  display: block;
  font-size: 20px;
  position: relative;
}
.section-header::before {
  width: 40%;
  display: block;
  position: absolute;
  content: "";
  background: black;
  height: 1px;
  left: 0;
  top: 50%;
}
.section-header::after {
  width: 40%;
  display: block;
  position: absolute;
  content: "";
  background: black;
  height: 1px;
  right: 0;
  top: 50%;
}
.option-card-content {
  line-height: 60px;
}
.option-card {
  height: 60px;
}
.text-content {
}
.slider {
  padding: 180px 100px;
}
.home {
  padding: 50px;
}
</style>
