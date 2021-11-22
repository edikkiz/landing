<template>
  <div class="modal-wrapper">
    <div class="modal">
      <div @click="close" class="modal-close">
        <img src="../assets/img/close-form-button.png" />
      </div>
      <div class="title">
        LET’S DISCUSS <br />
        YOUR BUSINESS CASE!
      </div>
      <div class="text">
        Everything is possible! We will analyze your existing situation,
        discover the bottlenecks and offer a solution that exactly matches your
        business case!
      </div>
      <div class="inputs">
        <div class="input-name">
          <label>First Name</label>
          <input placeholder="Klaus" type="text" />
        </div>
        <div class="input-name">
          <label>Last Name</label>
          <input placeholder="Voormann" type="text" name="" id="" />
        </div>
      </div>
      <div class="inputs">
        <div class="full-wrapper">
          <label>E–Mail</label>
          <input
            class="full"
            placeholder="klaus.voormann@email.de"
            type="text"
          />
        </div>
      </div>
      <div class="inputs">
        <div class="full-wrapper">
          <label>Some brief description or comments</label>
          <textarea
            class="text-box full"
            placeholder="My business case is completely different, so I want to discuss it with you."
          />
        </div>
      </div>
      <div class="privat-text">
        By pressing the “request a consultation” button you agree with
        <u><b>data protection</b></u> policy
      </div>
      <div class="button-modal-wrapper">
        <button @click="close" class="button-modal">
          <div class="button-modal-text">Request a Consultation</div>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Modal",
  methods: {
    close() {
      this.$emit("close");
    },
  },
};
</script>
