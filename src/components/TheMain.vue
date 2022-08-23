<template>
  <!-- Meet Barber -->
  <main>
    <section
      id="meet-barber"
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
    <!--  Section Services -->
    <section id="services">
      <div class="container">
        <h6 class="text-uppercase mt-5 fw-bold text-center">Men's grooming</h6>
        <h2 class="fw-bold text-center">Services</h2>

        <div class="row text-center py-5 justify-content-around">
          <div class="col-3 mt-4">
            <img
              src="../../public/images/avadabarbers-trimcut-icon-before.png"
              alt="Men's Grooming"
            />
            <h4 class="py-5 fw-bold">Trim & Cut</h4>
            <p class="grey-p">
              Avada Barbers are experts in the lickety split trim and hair cut.
              Quick but careful and ridiculously good looking.
            </p>
          </div>
          <div class="col-3 mt-4">
            <img
              src="../../public/images/avadabarbers-washndry-icon.png"
              alt="Wash & Dry"
            />
            <h4 class="py-5 fw-bold">Wash & Dry</h4>
            <p>
              Take a seat in our fine leather chairs, lean back and let us
              lather you a fresh head in a luxurious fashion.
            </p>
          </div>
          <div class="col-3 mt-4">
            <img
              src="../../public/images/avadabarbers-beardtrim-icon.png"
              alt="Beard Tidy"
            />
            <h4 class="py-5 fw-bold">Beard Tidy</h4>
            <p>
              Tame the tangles and untidy facial hairs like a gentleman with our
              Beard Tidy services from Avada Barbers.
            </p>
          </div>
        </div>

        <div class="d-flex align-items-center flex-column">
          <button class="mb-5 goldenrod_btn btn-general mt-2">
            Read about our services
          </button>
        </div>
      </div>

      <div class="triangle-transiction mt-5"></div>
    </section>
    <!-- Close Section Services -->

    <!-- SECTION PRODUCTS -->
    <section id="products">
      <div class="container"></div>
    </section>
    <!-- CLOSE SECTION PRODUCTS -->
  </main>
  <!-- CLOSE MAIN -->
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

h4 {
  font-size: 32px;
  color: $driftWood;
}

h6 {
  color: $driftWood;
  font-size: 14px;
  letter-spacing: 1px;
}

p {
  color: $gunbsmoke;
}

// SEZIONE MEET BARBER
#meet-barber {
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
// SECTION SERVICES

#services {
  h2 {
    color: $silverChalice;
  }

  img {
    max-height: 80px;
  }

  .triangle-transiction {
    background-image: linear-gradient(
        to bottom right,
        transparent 50%,
        $codGrayi 0
      ),
      linear-gradient(to top right, $codGrayi 50%, transparent 0);
  }
}
// SECTION PRODUCTS

#products {
  height: 500px;
  background-color: $codGrayi;
  width: 100%;
}
</style>