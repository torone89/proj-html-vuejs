<template>
  <header>
    <!-- NAVBAR -->
    <div class="container" id="section-0">
      <div>
        <b-navbar toggleable type="dark" variant="">
          <b-navbar-brand href="#">
            <img
              src="../../public/images/avadabarbers-logo-x1.png"
              alt="Logo"
              class="pointer p-0"
          /></b-navbar-brand>

          <b-navbar-toggle target="navbar-toggle-collapse" class="b-0">
            <template #default="{ expanded }">
              <b-icon icon="cart4" class="mx-4 fs-3"></b-icon>
              <b-icon v-if="expanded" icon="list" class="fs-3"></b-icon>
              <b-icon v-else icon="list" class="fs-3"></b-icon>
            </template>
          </b-navbar-toggle>

          <b-collapse id="navbar-toggle-collapse" is-nav>
            <b-navbar-nav class="ml-auto text-center">
              <!-- LOGICA PER GIRARE NELLE SEZIONI E STAMPO I DATI DELL'ARRAY MENUHAMBURGER -->
              <b-nav-item
                :href="`#section-${index}`"
                v-for="(menu, index) in menuHamburger"
                :key="index"
                >{{ menu }}</b-nav-item
              >
            </b-navbar-nav>
          </b-collapse>
        </b-navbar>
      </div>
      <!-- ClOSE NAVBAR -->
      <!-- JUMBOTRON -->

      <div id="jumbotron">
        <div class="row" id="section-1">
          <div
            class="
              col-6
              d-flex
              justify-content-center
              flex-column
              align-items-start
            "
          >
            <h1>Barber Shop</h1>
            <hr />
            <p class="fs-3 text-title">The Pinnacle of Male Grooming</p>
            <div>
              <button class="mt-5 goldenrod_btn btn-general">Learn More</button>
            </div>
          </div>
          <div class="col-6">
            <img
              src="../../public/images/avadabarbers_hero_focalmirror.png"
              alt="Jumbo Photo Hair Cut"
              class="img-fluid w-75"
            />
          </div>
        </div>
      </div>
      <!--  CLOSE JUMBOTRON -->
    </div>

    <!-- Buttons Fix-->
    <div id="buttons-fix">
      <button
        id="demos"
        class="white_btn pointer d-block border-0 rounded-3 mb-1 p-2"
      >
        <i class="fas fa-3x fa-folder-plus"></i>
        <p>Demos</p>
      </button>
      <button id="sale" class="white_btn pointer border-0 rounded-3">
        <i class="fas fa-dollar-sign pt-1"></i>
        <span class="fs-3 fw-bold number-sale p-0">39</span>
        <p>On Sale</p>
      </button>
    </div>
    <!-- CLOSE BUTTON FIX -->
  </header>
</template>

<script>
export default {
  name: "BaseHeader",
  props: { menuHamburger: Array },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";
header {
  background: url(../../public/images/avadabarbers-homepage-hero-bg.jpg);

  #jumbotron {
    h1 {
      font-size: 100px;
      font-weight: 900;
      color: $white;
    }
    hr {
      width: 60%;
      height: 10px;
      color: $goldenrod;
      opacity: 0.8;
    }
  }
  // BUTTON FIXED

  #buttons-fix {
    position: fixed;
    top: 20%;
    right: 5px;
    z-index: 2;
    font-size: 14px;
    .white_btn {
      width: 70px;
      height: 70px;
      color: $emperor;
    }
    #demos {
      i {
        color: $kashmirBlue;
      }
      p {
        font-size: 12px;
      }
    }
    #sale {
      i,
      .number-sale {
        color: $fluoGreen;
      }
      i {
        position: relative;
        top: -5px;
      }
      span {
        position: relative;
        top: 5px;
      }
      p {
        font-size: 12px;
        position: relative;
        top: -2px;
      }
    }
  }
}
</style>

