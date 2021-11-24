<template>
  <div class="row">
    <div class="col-1"></div>
    <div class="col-10 title Have-you-experienced">
      HAVE YOU EXPERIENCED ANY OF THESE ISSUES?
    </div>
  </div>
  
    <Carousel class="carousel"/>
</template>

<script>
import Carousel from "./Carousel.vue";

export default {
  components: { Carousel },
  name: "How-you-experienced",
}
</script>
