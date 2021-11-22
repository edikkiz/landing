<template>
  <div class="row">
    <div class="col-1"></div>
    <div class="col-10 title Have-you-experienced">
      HAVE YOU EXPERIENCED ANY OF THESE ISSUES?
    </div>
  </div>

  <div class="row">
    <div class="col-1"></div>
    <div class="col-11">
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
        <div class="card-info last">
          <div class="card-info-title">Inefficient truck load</div>
          <div class="card-info-text">
            Without dynamic truck load scheduling, your company misses up to 50%
            of the potential loading capability
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="row">
    <div class="col-1"></div>
    <div class="col-2 nav-buttons">
      <div class="prev-button">
        <img src="../assets/img/prev-button.png" />
      </div>
      <div class="next-button">
        <img src="../assets/img/next-button.png" />
      </div>
    </div>
    <div class="col-2"></div>
    <div class="col-2 selector-buttons">
      <div class="selector-button active">
        <img src="../assets/img/active-selector-dot.png" />
      </div>
      <div class="selector-button">
        <img src="../assets/img/selector-dot-2.png" />
      </div>
      <div class="selector-button">
        <img src="../assets/img/selector-dot-2.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "How-you-experienced",
};
</script>
