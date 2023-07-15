
<script>
// @ is an alias to /src

var file2 = require("@/assets/first1.webp");

export default {
  name: "HomeView",
  components: {
   
  },
  data: function () {
    return {
      
      file2,
      
    };
  },
};
</script>
<template>
  <div>
    <!-- Intro -->
    <section class="pt-2 pb-8">
      <div
        class="container min-h-[80vh] flex flex-col-reverse items-center gap-12 lg:flex-row"
      >
        <div class="flex flex-col gap-4 lg:basis-full">
          <div
            class="flex items-center gap-2 px-2 py-1 bg-[#FDDDDD] w-fit rounded-full"
          >
            <NuxtIcon name="Heart" filled class="text-lg" />
            <p>People trust us</p>
          </div>

          <h1 class="mb-4 text-5xl font-bold dark:text-white lg:leading-tight text-h3 text-start">
            We're <span class="text-red">Serious</span> For
            <span class="text-red">Food</span> &
            <span class="delivery">Delivery</span>.
          </h1>

          <p class="text-gray-100 dark:text-white text-start">
            Best cooks and best delivery guys all at your service. Hot tasty
            food will reach you in 60 minutes.
          </p>
          <SearchTextField />
        </div>

        <div class="grid lg:basis-full place-content-center">
          <v-img class="ml-10" :src="file2"></v-img>
        </div>
      </div>
    </section>

    <!-- Features -->
    <section
      class="flex flex-col gap-6 py-12 md:flex-row md:items-center md:gap-40"
    >
      <div>
        <img
          src="@/assets/first1.webp"
          alt="Chef holding food"
          loading="lazy"
        />
      </div>

      <div class="container flex flex-col max-w-4xl gap-6 ml-0">
        <h2 class="text-5xl font-bold dark:text-white lg:leading-tight">
          We are <span class="text-red">more</span> than
          <span class="text-yellow">multiple</span> service
        </h2>

        <p class="text-gray-100 dark:text-white">
          This is a type of restaurant which typically serves food and drink, in
          addition to light refreshments such as baked goods or snacks. The term
          comes from the french word meaning food.
        </p>

        <ul
          class="grid grid-cols-1 gap-4 font-medium md:grid-cols-2 dark:text-white"
        >
          <li class="flex items-center gap-2">
            <NuxtIcon name="shopping" filled class="text-3xl" />
            <p>Online Order</p>
          </li>

          <li class="flex items-center gap-2">
            <NuxtIcon name="24-hours" filled class="text-3xl" />
            <p>24/7 Service</p>
          </li>

          <li class="flex items-center gap-2">
            <NuxtIcon name="chef" filled class="text-3xl" />
            <p>Super Chef</p>
          </li>

          <li class="flex items-center gap-2">
            <NuxtIcon name="reserved" class="text-3xl text-red" />
            <p>Pre-Reservation</p>
          </li>

          <li class="flex items-center gap-2">
            <NuxtIcon name="restaurant" class="text-3xl text-yellow" />
            <p>Oragonized Foodhut Place</p>
          </li>

          <li class="flex items-center gap-2">
            <NuxtIcon name="clean" class="text-3xl text-red" />
            <p>Clean Kitchen</p>
          </li>
        </ul>

        <button
          class="px-6 py-2 text-white transition-opacity rounded-full bg-red w-fit hover:opacity-90"
        >
          About Us
        </button>
      </div>
    </section>

    <!-- Mobile Apps -->
    <section
      class="flex flex-col gap-6 py-12 md:flex-row-reverse md:items-center md:gap-40"
    >
      <div>
        <img
          src="@/assets/first1.webp"
          alt="Chef holding food"
          loading="lazy"
        />
      </div>

      <div class="container flex flex-col max-w-4xl gap-6 ml-0">
        <h2 class="text-5xl font-bold dark:text-white lg:leading-tight">
          It's Now <span class="text-red">More Easy</span> to
          <span class="text-yellow">Order</span> by Our Mobile App
        </h2>

        <p class="text-gray-100 dark:text-white">
          All you need to do is downlode one of the best delivery apps, make a
          and most companies are opting for mobile app devlopment for food
          delivery
        </p>

        <div class="flex gap-4">
          <a href="#" aria-label="Google Play">
            <img
              src="@/assets/first1.webp"
              alt="Google Play"
              loading="lazy"
            />
          </a>

          <a href="#" aria-label="App Store">
            <img
              src="@/assets/first1.webp"
              alt="App Store"
              loading="lazy"
            />
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped lang="scss">
  .delivery {
    @apply text-yellow relative after:bg-text-decore after:bg-no-repeat after:w-full after:h-3 after:-bottom-1 after:-left-1 after:absolute;
  }
</style>

<style>
  body,
  html {
    @apply scroll-smooth;
  }

  body {
    @apply bg-no-repeat bg-red-graident-light dark:bg-red-graident-dark bg-pale-white dark:bg-gray-300 transition-colors font-poppins;
  }

  .nuxt-icon svg {
    @apply m-0;
  }
</style>