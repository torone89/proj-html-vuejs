<template>
  <header>
    <div class="container">
      <!-- JUMBOTRON -->

      <div id="jumbotron">
        <div class="row">
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
        class="white_btn pointer d-block border-0 rounded-3 mb-1"
      >
        <i class="fas fa-3x fa-folder-plus"></i>
        <p>Demos</p>
      </button>
      <button id="sale" class="white_btn pointer border-0 rounded-3">
        <i class="fas fa-dollar-sign"></i>
        <span class="fs-3 fw-bold number-sale">39</span>
        <p>On Sale</p>
      </button>
    </div>
    <!-- CLOSE BUTTON FIX -->
  </header>
</template>

<script>
export default {
  name: "BaseHeader",
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
  // BUTONI FIXED

  #buttons-fix {
    position: fixed;
    top: 20%;
    right: 5px;
    z-index: 2;
    font-size: 14px;
    .white_btn {
      width: 70px;
      height: 70px;
      outline: none;
      color: $emperor;
    }
    #demos {
      i {
        color: $kashmirBlue;
      }
    }
    #sale {
      i,
      .number-sale {
        color: $fluoGreen;
      }
      i {
        position: relative;
        top: -10px;
      }
    }
  }
  // --Top right fixed buttons
}
</style>