<template>
  <!-- Meet Barber -->
  <main>
    <section
      id="meet-barber"
      class="d-flex flex-column justify-content-around align-items-center"
    >
      <h6 class="text-uppercase mt-5 mb-4 fw-bold p-3">Award winning</h6>
      <h2 class="mb-3 fw-bold">Pro barbers</h2>
      <button class="mb-5 goldenrod_btn btn-general mt-2" id="section-1">
        Meet your new barber
      </button>
      <div class="triangle-transiction mt-5"></div>
    </section>
    <!-- /Close MeetBarber -->
    <!--  Section Services -->
    <sectionServices />

    <!-- Close Section Services -->

    <!-- SECTION PRODUCTS -->
    <sectionProduct />

    <!-- SECTION REVIEWS+ RELATIVE SHAVING -->

    <section id="reviews">
      <!-- POSITION RELATIVE SHAVING -->
      <div class="container mb-5 position-shaving" id="section-4">
        <div class="row justify-content-center">
          <div
            id="shaving-butter-img"
            class="
              col-4
              d-flex
              align-items-center
              justify-content-center
              bg-shave
            "
          >
            <img
              src="../../public/images/shaving_butter-800x800.png"
              alt="shaving butter"
              class="img-fluid w-75"
            />
          </div>

          <div class="col-6 bg-shave px-5">
            <h6 class="fw-bold mt-5 text-uppercase">
              This month featured product
            </h6>
            <h2 class="fw-bold">Shaving Butter</h2>
            <p class="mt-5">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Pellentesque laoreet enim est, vel molestie dolor ultrices ut.
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            </p>
            <button class="mb-5 goldenrod_btn btn-general">Buy now</button>
          </div>
        </div>
        <!-- CLOSE POSITION SHAVING-BUTTER -->
      </div>
      <!-- SECTION REVIEW -->
      <sectionReview />

      <!-- Blog posts -->
      <sectionBlog />
    </section>
  </main>
  <!-- CLOSE MAIN -->
</template>

<script>
import SectionBlog from "./SectionBlog.vue";
import SectionReview from "./SectionReview.vue";
import SectionServices from "./SectionServices.vue";
import SectionProduct from "./SectionProduct.vue";
export default {
  name: "TheMain",
  components: {
    SectionBlog,
    SectionReview,
    SectionServices,
    SectionProduct,
  },
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

// GENERAL

// SEZIONE MEET BARBER
#meet-barber {
  background: $bgMeetBarber;
  .triangle-transiction {
    background-image: linear-gradient(
        to bottom right,
        transparent 50%,
        #ffffff 0
      ),
      linear-gradient(to top right, #ffffff 50%, transparent 0);
  }
}

// SECTION REVIEWS
#reviews {
  .position-shaving {
    position: relative;
    top: -50px;

    h6 {
      font-size: 14px;
    }

    .bg-shave {
      border-top: 3px solid $goldenrod;
      background-color: $codGrayi;
    }
  }
  #shaving-butter-img {
    background: $bgShavingButter;
  }
}
</style>