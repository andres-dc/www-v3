<template>
  <div
    class="container-sm min-h-full font-lato flex-1 flex flex-col place-content-center items-center mx-10 text-left"
  >
    <div class="lg:w-1/2">
      <h1 class="text-3xl m-3">
        I'm
        <span class="font-titillium font-bold text-name">
          Andrés Del Carpio
        </span>
      </h1>
      <p class="text-xl m-3">
        Full-stack developer, student &#38; technical writer.
      </p>
    </div>
    <Logos />
  </div>
</template>

<script>
import Logos from '../components/Logos';

export default {
  name: 'Home',
  components: {
    Logos,
  },
  created() {
    document.title = process.env.VUE_APP_TITLE;
  },
};
</script>
