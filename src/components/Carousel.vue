<template>
  <carousel
    v-if="width > 768"
    :snapAlign="start"
    :itemsToScroll="1"
    :items-to-show="2.75"
  >
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

  <carousel
    v-if="width <= 768 && width > 425"
    :snapAlign="start"
    :items-to-show="1.95"
  >
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

  <carousel v-if="width <= 425" :snapAlign="start" :items-to-show="1">
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
      start: "start",
      width: window.outerWidth,
    };
  },
};
</script>

<style lang="scss" scoped>
.carousel {
  width: 1188px;
  margin-left: 95px;
  margin-bottom: 178px;
}

.cards {
  width: 435px;
  display: flex;
  .card-info {
    width: 420px;
    height: 368px;
    margin-right: 15px;
    padding: 0 37px 0 38px;
    object-fit: contain;
    box-shadow: 0 10px 30px 0 rgba(8, 61, 119, 0.25);
    background-color: $twilight-blue;
    .card-info-title {
      text-align: start;
      padding-top: 67px;
      font-family: $OpenSans;
      height: 50px;
      margin: 0 0px 22px 0px;
      font-size: 21px;
      font-weight: bold;
      line-height: 25px;
      letter-spacing: -0.53px;
      color: $white;
    }
    .card-info-text {
      text-align: start;
      padding-top: 67px;
      font-family: $OpenSans;
      font-size: 17px;
      font-weight: 400;
      font-stretch: normal;
      font-style: normal;
      line-height: normal;
      letter-spacing: -0.43px;
      color: $white;
      opacity: 0.8;
    }
  }
}
@media (max-width: 768px) {
  .carousel {
    width: 768px;
    margin-left: 66px;
  }

  .cards {
    width: 375px;
    margin-left: -25px;
    .card-info {
      margin-right: 0;
      padding: 87px 15px;
      width: 375px;
      .card-info-title {
        padding-top: 0;
      }
      .card-info-text {
        padding-top: 0;
        font-size: 15px;
      }
    }
  }
}
@media (max-width: 426px) {
  .carousel {
    width: 375px;
    margin-left: 0px;
  }

  .cards {
    width: 100%;
    margin-left: 0px;
    .card-info {
      margin-right: 0;
      padding: 91px 30px;
      width: 375px;
      .card-info-title {
        padding-top: 0;
      }
      .card-info-text {
        padding-top: 0;
        font-size: 15px;
      }
    }
  }

}
</style>