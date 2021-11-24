<template>
  <carousel v-if="width > 768" :items-to-show="2.75">
    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">
            Overwhelming and <br />
            inaccurate paperwork
          </div>
          <div class="card-info-text">
            Most documents, such as orders, invoices, contracts, etc. are stored
            in folders on endless shelves. They are never easy to find.
            Moreover, due to human factor, crucial mistakes take place that cost
            your company much time to solve, but also drain your budget.
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">
            Manual order management <br />
            based on phone calls and emails
          </div>
          <div class="card-info-text">
            Do your clients call you just to find out that the necessary product
            is currently out of stock? You waste resources by not providing them
            with actual information about your available inventory online
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>

  <carousel v-if="width <= 768 && width > 425" :items-to-show="1.95">
    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">
            Overwhelming and <br />
            inaccurate paperwork
          </div>
          <div class="card-info-text">
            Most documents, such as orders, invoices, contracts, etc. are stored
            in folders on endless shelves. They are never easy to find.
            Moreover, due to human factor, crucial mistakes take place that cost
            your company much time to solve, but also drain your budget.
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">
            Manual order management <br />
            based on phone calls and emails
          </div>
          <div class="card-info-text">
            Do your clients call you just to find out that the necessary product
            is currently out of stock? You waste resources by not providing them
            with actual information about your available inventory online
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>

  <carousel v-if="width < 425" :items-to-show="1">
    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">
            Overwhelming and <br />
            inaccurate paperwork
          </div>
          <div class="card-info-text">
            Most documents, such as orders, invoices, contracts, etc. are stored
            in folders on endless shelves. They are never easy to find.
            Moreover, due to human factor, crucial mistakes take place that cost
            your company much time to solve, but also drain your budget.
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">
            Manual order management <br />
            based on phone calls and emails
          </div>
          <div class="card-info-text">
            Do your clients call you just to find out that the necessary product
            is currently out of stock? You waste resources by not providing them
            with actual information about your available inventory online
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <slide :key="slide">
      <div class="cards">
        <div class="card-info">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";

export default {
  name: "App",
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
  data() {
    return {
      width: window.outerWidth,
    };
  },
};
</script>