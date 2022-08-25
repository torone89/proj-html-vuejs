<template>
  <footer class="text-center">
    <!-- FOOTER TOP -->
    <div id="footer-top" class="container py-5">
      <div class="row" id="section-6">
        <div class="col-4">
          <img
            src="../../public/images/avadabarbers_footer_shop_image-400x312.png"
            alt="footer shop"
          />
          <button class="mt-4 goldenrod_btn btn-general">
            Shop our range now
          </button>
        </div>
        <div class="col-4 d-flex align-items-center flex-column">
          <!-- FOOTER INFO -->
          <ul>
            <li>
              <img
                src="../../public/images/avadabarbers-logo-x2-200x70.png"
                alt="logo"
                class="pt-4 mb-5"
              />
            </li>
            <li class="d-block grey-p">{{ footerInfo.name }}</li>
            <li class="d-block">{{ footerInfo.address }}</li>
            <li class="d-block grey-p">{{ footerInfo.city }}</li>
            <li class="d-block grey-p">{{ footerInfo.email }}</li>
            <li class="d-block grey-p mb-4">{{ footerInfo.number }}</li>
            <li class="text-uppercase fw-bold mt-5"><h5>Follow us</h5></li>
          </ul>
          <ul class="pt-3">
            <!-- LOGICA PER GIARE NELL'ARRAY -->
            <li
              v-for="(social, index) in socials"
              :key="index"
              class="d-inline-block px-2"
            >
              <a href="#"><i :class="`fab fa-${social}`"></i></a>
            </li>
          </ul>
        </div>
        <div class="col-4">
          <img
            src="../../public/images/avadabarbers_footer_appointment_image-400x312.png"
            alt="footer apponintment"
          />
          <button class="mt-4 goldenrod_btn btn-general">
            Book your appointment
          </button>
        </div>
      </div>
    </div>
    <!-- /CLOSE FOOTER TOP-->
    <!-- FOOTER BOTTOM -->

    <div
      id="footer-bottom"
      class="d-flex justify-content-center align-items-center"
    >
      <p class="m-0">
        <i class="far fa-copyright"></i> Copyright 2012 - 2020 | Avada Theme by
        ThemeFusion | All Rights Reserved | Powered by WordPress
      </p>
      <!-- BOTTONE FIX PER TORNARE A INIZIO PAGINA (top) -->
      <a href="#top"><i class="fas fa-chevron-up"></i></a>
    </div>

    <!-- CLOSE FOOTER BOTTOM -->
  </footer>
</template>

<script>
export default {
  name: "BaseFooter",
  data() {
    return {
      socials: ["facebook-f", "twitter", "youtube", "instagram"],
    };
  },
  props: {
    footerInfo: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

footer {
  background: $codGray;
  img {
    max-width: 100%;
  }
  // FOOTER TOP
  #footer-top {
    li {
      color: $emperor;
      opacity: 0.7;
      h5 {
        color: $goldenrod;
      }
    }
  }

  // FOOTER BOOTTOM
  #footer-bottom {
    height: 100px;
    background: $footerBottom;
    p {
      color: $gunbsmoke;
      opacity: 0.4;
      font-size: 14px;
    }
    a {
      bottom: 0;
      right: 2%;
      width: 45px;
      height: 30x;
      line-height: 30px;
      position: fixed;

      color: $ebb;
      background: $mineShaft;
    }
  }
}
</style>