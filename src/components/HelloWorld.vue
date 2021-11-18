<template>
  <div class="container">
    <div class="row row1">
      <header>
        <div class="col-3"></div>

        <div class="navbar col-6">
          <div class="navbar-elem">Benefits</div>
          <div class="navbar-elem">Advantages</div>
          <div class="navbar-elem">Achievements</div>
        </div>

        <div class="col-1"></div>
        <div class="language col-2">
          <div class="language-elem">DE</div>
          <div class="language-elem active">EN</div>
        </div>
      </header>
    </div>
    <div class="row">
      <div class="col-1"></div>
      <div class="LOGISTICS-MANAGEMENT col-8">
        LOGISTICS MANAGEMENT SOFTWARE DEVELOPMENT
      </div>
    </div>
    <div class="row">
      <div class="col-1"></div>
      <div class="col-7 first-text">
        We solve transportation and stock management problems for Factories,
        Manufacturers, Carriers, Resellers, E-commerce and even more. Any issue
        can be solved with smart digitalization.
      </div>
    </div>
    <div class="row">
      <div class="col-4"></div>
      <div class="col-4">
        <div class="button-desk-shadow">
          <button class="button-desk">
            <div class="button-desk-text">Request a free consultation</div>
          </button>
        </div>
      </div>
    </div>
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
              Most documents, such as orders, invoices, contracts, etc. are
              stored in folders on endless shelves. They are never easy to find.
              Moreover, due to human factor, crucial mistakes take place that
              cost your company much time to solve, but also drain your budget.
            </div>
          </div>
          <div class="card-info">
            <div class="card-info-title">
              Manual order management <br />
              based on phone calls and emails
            </div>
            <div class="card-info-text">
              Do your clients call you just to find out that the necessary
              product is currently out of stock? You waste resources by not
              providing them with actual information about your available
              inventory online
            </div>
          </div>
          <div class="card-info">
            <div class="card-info-title">Inefficient truck load</div>
            <div class="card-info-text">
              Without dynamic truck load scheduling, your company misses up to
              50% of the potential loading capability
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
    <div class="row">
      <div class="col-2"></div>
      <div class="col-4 second-text">
        Expenses reduction after implementing logistics management software!
      </div>
      <div class="col-4 procents">49,2%</div>
      <div class="col-2"></div>
    </div>
    <div class="row">
      <div class="col-1"></div>
      <div class="col-7 HOW-CAN-YOU-BENEFIT">
        HOW CAN YOU BENEFIT FROM <br />
        CUSTOM LOGISTICS SOFTWARE?
      </div>
    </div>
    <div class="row">
      <div class="col-6 notation-block">
        <div class="notation-wrapper">
          <div class="notation-icone">
            <img src="../assets/img/notation/group-1.png" />
          </div>
          <div>
            <div class="notation-title">Customized to your needs</div>
            <div class="notation-text">
              A software is developed exclusively with your needs and plans in
              mind. This enables to solve unique problems efficiently
            </div>
          </div>
        </div>
      </div>
      <div class="col-6 notation-block-right">
        <div class="notation-wrapper">
          <div class="notation-icone">
            <img src="../assets/img/notation/group-2.png" />
          </div>
          <div>
            <div class="notation-title">Short-term ROI</div>
            <div class="notation-text">
              You will experience the first returns right in the first month
              after integrating the system in your current processes
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-6 notation-block">
        <div class="notation-wrapper">
          <div class="notation-icone">
            <img src="../assets/img/notation/group-3.png" />
          </div>
          <div>
            <div class="notation-title">Predictable scalability</div>
            <div class="notation-text">
              A custom system grows along with your business since your company
              goals are taken into account in the development process
            </div>
          </div>
        </div>
      </div>
      <div class="col-6 notation-block-right">
        <div class="notation-wrapper">
          <div class="notation-icone">
            <img src="../assets/img/notation/group-4.png" />
          </div>
          <div>
            <div class="notation-title">Improve, not rebuild</div>
            <div class="notation-text">
              Custom software supports and improves your running processes
              step-by-step. Your current system keeps working
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-4"></div>
      <div class="col-4 YOUR-BUSINESS-CASE">
        YOUR BUSINESS CASE <br />
        IS COMPLETELY DIFFERENT?
        <p>LET’S DISCUSS</p>
      </div>
    </div>
    <div class="row">
      <div class="col-4"></div>
      <div class="col-4">
        <div class="button-desk-shadow">
          <button class="button-desk">
            <div class="button-desk-text">Fill in the contact form</div>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss"></style>
