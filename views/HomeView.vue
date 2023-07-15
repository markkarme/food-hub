<template>
  <v-app class="background-color">
    <div>
      <v-row>
        <v-col cols="2" :sm="6" :md="2">
          <v-img class="ml-10" width="150" height="150" :src="file1"></v-img>
        </v-col>
        <v-col class="mt-6" cols="8">
          <SearchTextField />
        </v-col>
      </v-row>
    </div>
    <div class="container">
      <v-row>
        <v-col class="d-flex align-center ml-4">
          <div class="flex flex-col gap-4 lg:basis-full">
            <div
              class="flex items-center gap-2 px-2 py-1 bg-[#FDDDDD] w-fit rounded-full"
            >
              <v-chip
                class="d-flex justify-center text-color ml-4"
                color="red"
                text-color="black"
                style="width: 135px"
                prepend-icon="mdi-heart"
              >
                People trust us
              </v-chip>
            </div>

            <h1
              class="mb-4 text-5xl font-bold dark:text-white lg:leading-tight text-h3 text-start text-h3"
            >
              We're <span class="text-red">Serious</span> For
              <span class="text-red">Food</span> &
              <span class="delivery text-yellow">Delivery</span>.
            </h1>

            <p class="text-gray-100 dark:text-white text-start">
              Best cooks and best delivery guys all at your service. Hot tasty
              food will reach you in 60 minutes.
            </p>
            
            <v-col cols="2">
              
            </v-col>
          </div>
          
        </v-col>
        <v-col cols="12" md="6" lg="6" xl="6" sm="6">
          <v-img class="ml-10" :src="file2"></v-img>
        </v-col>
      </v-row>
    </div>
    <div>
      <v-row class="">
        <v-col class="justify-start mr-16" cols="12" sm="6">
          <v-img class="mr-16" :src="file3"></v-img>
        </v-col>
        <v-col class="d-flex align-center ml-16">
          <div class="flex flex-col gap-4 lg:basis-full ">
            <h1
              class="mb-4 text-5xl font-bold dark:text-white lg:leading-tight text-h3 text-start text-h3"
            >
              We are <span class="text-red">more</span> than
              <span class="text-yellow">multiple</span> service
            </h1>

            <p class="text-gray-100 dark:text-white text-start">
              This is a type of restaurant which typically serves food and
              drink, in addition to light refreshments such as baked goods or snacks. The term comes from the french word
                meaning food.
            </p>
            <v-row class="mt-4 ml-1">
              <v-col>
                <div
                  class="d-flex justify-start mb-4"
                  v-for="(elemnt, i) in 3"
                  :key="i"
                >
                  <v-icon class="font-weight-bold mr-2" size="25">{{
                    leftDataIcon[i]
                  }}</v-icon>
                  <p class="text-h6 text-start">{{ leftDataText[i] }}</p>
                </div>
              </v-col>
              <v-col>
                <div
                  class="d-flex justify-start mb-4"
                  v-for="(elemnt, i) in 3"
                  :key="i"
                >
                  <v-icon class="font-weight-bold mr-2" size="30">{{
                    rightDataIcon[i]
                  }}</v-icon>
                  <p class="text-h6">{{ rightDataText[i] }}</p>
                </div>
              </v-col>
            </v-row>
            <v-btn color="red" class="d-flex justify-start" rounded="xl"
              >About us</v-btn
            >
          </div>
          
        </v-col>
      </v-row>
    </div>
    <div class="background-color2">
      <v-row>
        <v-col class="flex justify-start ml-4 mr-4">
          <v-card-item>
            <v-row class="ma-4">
              <p class="font-weight-bold mr-2 text-h2">It's Now</p>
              <p class="font-weight-bold mr-2 text-h2 text-red">More Easy</p>
              <p class="font-weight-bold mr-2 text-h2">to</p>
              <p class="font-weight-bold mr-2 text-h2 text-yellow">order</p>
              <p class="font-weight-bold mr-2 text-h2">by</p>
            </v-row>
            <p class="ml-4 font-weight-bold text-h3 d-flex justify-start">
              Our Mobile App
            </p>
            <p class="ma-4 text-start">
              All you need to do is downlode one of the best delivery apps, make
              a and most companies are opting
            </p>
            <p class="ml-4 text-start">
              for mobile app devlopment for food delivery
            </p>
            <div class="d-flex justify-start ml-4">
              <v-btn
                class="my-button mb-4 mt-4 mr-4"
                :ripple="false"
                width="170"
                height="55"
                variant="text"
              ></v-btn>
              <v-btn
                class="my-button2 mb-4 mt-4 mr-4"
                :ripple="false"
                width="170"
                height="55"
                variant="text"
              ></v-btn>
            </div>
          </v-card-item>
        </v-col>
        <v-col cols="12" sm="5">
          <v-img class="ml-12" :src="file4"></v-img>
        </v-col>
      </v-row>
    </div>
    <v-footer class="background-color2">
      <v-row>
        <v-col class="flex" cols="4">
          <v-btn
            class="my-button3 mb-4 mt-4 mr-4 "
            :ripple="false"
            height="100"
            width="170"
            variant="text"
          ></v-btn>
          <p class="text-start">
            The perfect place for you to find your next amazing recipe! Start
            exploring your next meal now!
          </p>
          <v-row class="justify-center mt-4 pl-4 mb-3">
            <v-icon color="yellow mr-4" size="35">mdi-facebook</v-icon>
            <v-icon color="yellow mr-4" size="35">mdi-instagram</v-icon>
            <v-icon color="yellow " size="35">mdi-twitter</v-icon>
          </v-row>
        </v-col>
        <v-col class="flex">
          <p class="text-red text-h4 mb-4 text-start">About us</p>
          <v-btn
            v-for="(elemnt, i) in 4"
            :key="i"
            variant="text"
            class="footer-btn d-flex text-start"
            :ripple="false"
            >{{ aboutUsFooter[i] }}</v-btn
          >
        </v-col>
        <v-col>
          <p class="text-red text-h4 mb-4 text-start">Company</p>
          <v-btn
            v-for="(elemnt, i) in 4"
            :key="i"
            variant="text"
            class="footer-btn d-flex text-start"
            :ripple="false"
            >{{ CompanyFooter[i] }}</v-btn
          >
        </v-col>
        <v-col cols="4">
          <p class="text-red text-h4 text-start">Newsletter</p>
          <p class="text-start mt-4">
            Join our newsletter and get amazing recipes that will make lose your
            mind!. What are you waiting for? Can't you hear your belly? Join us
            now!
          </p>
          <v-row class="mt-4">
            <v-text-field
              placeholder="Email"
              rounded="xl"
              color="grey"
              variant="solo-filled"
              class="my-text-field mr-10 ml-2"
            ></v-text-field>
            <v-btn color="red" rounded="xl" class="mr-10 mt-2">subscribe</v-btn>
          </v-row>
        </v-col>
      </v-row>
    </v-footer>
  </v-app>
</template>

<script>
// @ is an alias to /src
import SearchTextField from "../components/searchTextField.vue";
var file1 = require("@/assets/food-logo.png");
var file2 = require("@/assets/first1.webp");
var file3 = require("@/assets/secound.webp");
var file4 = require("@/assets/third.webp");
export default {
  name: "HomeView",
  components: {
    SearchTextField,
  },
  data: function () {
    return {
      file1,
      file2,
      file3,
      file4,
      leftDataIcon: [
        "mdi-cellphone",
        "mdi-chef-hat",
        "mdi-silverware-fork-knife",
      ],
      leftDataText: ["Online Order", "Super Chef", "Oragonized Foodhut Place"],
      rightDataIcon: [
        "mdi-clock-time-five-outline",
        "mdi-waveform",
        "mdi-water-outline",
      ],
      rightDataText: ["24/7 Service", "Pre-Reservation", "Clean Kitchen"],
      aboutUsFooter: ["About Us", "Service Us", "Contact", "Company"],
      CompanyFooter: ["Partnership", "Terms of Use", "Privacy", "Sitemap"],
    };
  },
};
</script>

<style scoped>
.background-color {
  /* background:  #FEEFEF; */
  background: linear-gradient(to left, #feefef, #feefef);
}
.background-color2 {
  background: #fef9f9;
}

.my-button {
  background: url("@/assets/app store.png") no-repeat center center;
  background-size: cover;
}
.my-button2 {
  background: url("@/assets/google play.png") no-repeat center center;
  background-size: cover;
}

.my-button3 {
  background: url("@/assets/Food-Hut-Logo-Dark.svg") no-repeat center center;
  background-size: cover;
}
.footer-btn {
  text-transform: none;
}
.footer-btn:hover {
  box-shadow: none;
  color: orange;
}

.my-text-field {
  width: 50px;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

@media (max-width: 768px) {
  .container {
    flex-direction: column;
  }
}
</style>
