<template>
  <!-- Find new barber -->
  <section
    id="new-barber"
    class="d-flex flex-column justify-content-around align-items-center"
  >
    <h6 class="text-uppercase mt-5 mb-4 fw-bold p-3">Award winning</h6>
    <h2 class="mb-3 fw-bold">Pro barbers</h2>
    <button class="mb-5 goldenrod_btn btn-general mt-2">
      Meet your new barber
    </button>
    <div class="triangle-transiction mt-5"></div>
  </section>
  <!-- /Close MeetBarber -->
</template>

<script>
export default {
  name: "TheMain",
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

// GENERAL
h2 {
  font-size: 80px;
  color: $starWhite;
}

h6 {
  color: $goldenrod;
  font-size: 14px;
  letter-spacing: 1px;
}

// SEZIONE NEW BARBER
#new-barber {
  background: url(../../public/images/avadabarbers-about-introbackground.jpg);
  .triangle-transiction {
    background-image: linear-gradient(
        to bottom right,
        transparent 50%,
        #ffffff 0
      ),
      linear-gradient(to top right, #ffffff 50%, transparent 0);
  }
}
</style>