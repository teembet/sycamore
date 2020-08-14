<template>
  <div>
    <div class="footer">
      <div class="contain">
        <div class="col-large">
          <img src="../assets/footer.png" alt="" />
          <p>
            At Sycamore, our primary objective is to create more opportunities
            to get you financially empowered. Follow us on social media
            Platforms, as we make this objective a reality.
          </p>
          <br />
          <v-btn
            depressed
            style=" text-transform:none;border-radius:20px;"
            dark
            color="#63C132"
            >Download our brochure
            <v-icon style="margin-left:10px;font-size:13px" dark
              >mdi-arrow-right</v-icon
            ></v-btn
          >
        </div>
        <div class="col">
          <h1>Company</h1>
          <ul>
            <li>About Us</li>
            <li>Contact Us</li>
            <li>FAQ</li>
            <li>Blog</li>
            <li>Food Store</li>
          </ul>
        </div>
        <div class="col">
          <h1>Products</h1>
          <ul>
            <li>Invest</li>
            <li>Borrow</li>
            <li>Advisory</li>
          </ul>
        </div>
        <div class="col">
          <h1>Legal</h1>
          <ul>
            <li>Privacy Policy</li>
            <li>Terms</li>
          </ul>
        </div>
        <div class="col">
          <h1>Company</h1>
          <ul>
            <li>
              <v-icon style="font-size:20px;margin-right:5px;" color="#63C132"
                >mdi-map-marker</v-icon
              >15, Modupe Johnson Crescent,Surulere, Lagos.
            </li>
            <li>
              <v-icon style="font-size:20px;margin-right:5px;" color="#63C132"
                >mdi-phone-plus</v-icon
              >+2348097341810
            </li>
          </ul>
        </div>
        <div class="clearfix"></div>
      </div>
    </div>
    <v-footer dark padless>
      <v-card class="flex" flat tile>
        <v-card-title style="background:#4D4D4D">
          <strong style="width:800px;font-size:12px" class="subheading"
            >Sycamore is authorized and regulated by the Money Lenders Act Cap
            52. The Sycamore brand is a property of Sycamore Integrated
            Solutions Limited. © Copyrights, All right reserved by
            Sycamore</strong
          >

          <v-spacer></v-spacer>

          <v-btn v-for="icon in icons" :key="icon" class="mx-4" dark icon>
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-title>
      </v-card>
    </v-footer>
  </div>
</template>

<script>
export default {
  name: "footer",
};
</script>

<style>
.footer {
  width: 100%;
  position: relative;
  height: 400px;
  background-color: #e8f2e9;
  padding: 50px 30px;
}
.footer .col {
  width: 15%;
  height: auto;
  float: left;
  box-sizing: border-box;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  padding: 0px 20px 20px 20px;
}
.footer .col-large {
  width: 40%;
  height: auto;
  float: left;
  box-sizing: border-box;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  padding: 0px 20px 20px 20px;
}
.footer .col-large h1 {
  margin-bottom: 10px;
  padding: 0;
  font-family: inherit;
  font-size: 13px;
  line-height: 19px;
  padding: 20px 0px 5px 0px;
  color: rgb(26, 26, 26);
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 0.25em;
}
.footer .col-large p {
  margin: 0;
  padding: 0;
  font-family: inherit;
  font-size: 13px;
  line-height: 19px;
  padding: 20px 0px 5px 0px;
  color: #002d04;
  letter-spacing: 0.1em;
}
.footer .col h1 {
  margin-bottom: 20px;
  padding: 0;
  font-family: inherit;
  font-size: 13px;
  line-height: 17px;
  padding: 20px 0px 5px 0px;
  color: #002d04;
  font-weight: bold;
  text-transform: uppercase;
  letter-spacing: 0.25em;
}
.footer .col ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
}
.footer .col ul li {
  color: #1d1d1d;
  font-size: 13px;
  font-family: inherit;
  padding: 5px 0px 5px 0px;
  cursor: pointer;
  transition: 0.2s;
  -webkit-transition: 0.2s;
  -moz-transition: 0.2s;
}
.social ul li {
  display: inline-block;
  padding-right: 5px !important;
}

.footer .col ul li:hover {
  color: #df3b3b;
  transition: 0.1s;
  -webkit-transition: 0.1s;
  -moz-transition: 0.1s;
}
.clearfix {
  clear: both;
}
.store {
  color: white;
}
.social-media {
  color: white;
}
.social-media-store {
  padding: 0 5%;
}
.footer-bottom-div {
  border-top: 1px solid white;
  border-bottom: 1px solid white;
  text-align: center;
  display: block;
  color: white;
  background: #252525;
  height: 70px;
  &-text {
    line-height: 70px;
  }
}
@media only screen and (min-width: 1280px) {
  .contain {
    width: 1200px;
    margin: 0 auto;
  }
}
@media only screen and (max-width: 1139px) {
  .contain .social {
    width: 1000px;
    display: block;
  }
  .social h1 {
    margin: 0px;
  }
}
@media only screen and (max-width: 950px) {
  .footer .col {
    width: 33%;
  }
  .footer .col h1 {
    font-size: 14px;
  }
  .footer .col ul li {
    font-size: 13px;
  }
}
@media only screen and (max-width: 500px) {
  .footer .col {
    width: 100%;
  }
  .footer .col h1 {
    font-size: 14px;
  }
  .footer .col ul li {
    font-size: 13px;
  }
}
@media only screen and (max-width: 340px) {
  .footer .col {
    width: 100%;
  }
}
</style>
