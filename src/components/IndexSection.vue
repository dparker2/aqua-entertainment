<template>
  <section class="relative bg-cover py-20 md:py-32 mb-10">
    <background-image :img="img" />
    <div class="relative z-10 mx-4 sm:mx-10 md:mx-20">
      <div class="font-black text-4xl sm:text-6xl md:text-8xl uppercase">{{ title }}</div>
      <div class="md:w-1/2 max-w-3xl">
        <div>{{ text }}</div>
        <div class="text-center">
          <a :href="learn">
            <button class="mt-10 border-2 px-4 text-xl hover:bg-black">Learn More</button>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BackgroundImage from "~/components/BackgroundImage.vue";
export default {
  props: {
    img: String,
    title: String,
    text: String,
    learn: String
  },
  components: {
    BackgroundImage
  }
};
</script>
