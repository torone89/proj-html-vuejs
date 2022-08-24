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

        <ul class="row text-center py-5 justify-content-around">
          <li class="col-3 mt-4">
            <img
              src="../../public/images/avadabarbers-trimcut-icon-before.png"
              alt="Men's Grooming"
            />
            <h4 class="py-5 fw-bold">Trim & Cut</h4>
            <p>
              Avada Barbers are experts in the lickety split trim and hair cut.
              Quick but careful and ridiculously good looking.
            </p>
          </li>
          <li class="col-3 mt-4">
            <img
              src="../../public/images/avadabarbers-beardtrim-icon.png"
              alt="Wash & Dry"
            />
            <h4 class="py-5 fw-bold">Wash & Dry</h4>
            <p>
              Take a seat in our fine leather chairs, lean back and let us
              lather you a fresh head in a luxurious fashion.
            </p>
          </li>
          <li class="col-3 mt-4">
            <img
              src="../../public/images/avadabarbers-washndry-icon.png"
              alt="Beard Tidy"
            />
            <h4 class="py-5 fw-bold">Beard Tidy</h4>
            <p>
              Tame the tangles and untidy facial hairs like a gentleman with our
              Beard Tidy services from Avada Barbers.
            </p>
          </li>
        </ul>

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
    <section
      id="products"
      class="
        d-flex
        flex-column
        justify-content-around
        align-items-center
        text-center
        py-5
      "
    >
      <div class="container">
        <h6 class="text-uppercase fw-bold mt-5 text-center">
          We have you covered
        </h6>
        <h2 class="mb-5 fw-bold text-center">Avada Grooming Products</h2>
        <ul class="row maxh-400">
          <li class="col-3">
            <img
              src="../../public/images/brush_dark-400x400.png"
              alt="Dark brush"
            />
            <h4 class="fw-bold">Brush</h4>
            <p class="text-gold"><span class="fs-4">$</span>15.00</p>
          </li>
          <li class="col-3">
            <img
              src="../../public/images/scissors-400x400.png"
              alt="scissors"
            />
            <h4 class="fw-bold">Scissors</h4>
            <p class="text-gold"><span class="fs-4">$</span>85.00</p>
          </li>
          <li class="col-3">
            <img
              src="../../public/images/hot_oil_dark-400x400.png"
              alt="hot oil"
            />
            <h4 class="fw-bold">Hot Oil</h4>
            <p class="text-gold"><span class="fs-4">$</span>15.00</p>
          </li>
          <li class="col-3">
            <img
              src="../../public/images/straight_razor_dark-400x400.png"
              alt="straight razor"
            />
            <h4 class="fw-bold">Straight Razor</h4>
            <p class="text-gold"><span class="fs-4">$</span>30.00</p>
          </li>
        </ul>
      </div>
      <button class="mb-5 goldenrod_btn btn-general">
        Shop our product range
      </button>
    </section>
    <!-- CLOSE SECTION PRODUCTS -->

    <!-- SECTION REVIEWS -->
    <section id="reviews">
      <!-- POSITION RELATIVE SHAVING -->
      <div class="container mb-5 position-shaving">
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
      <div class="container text-center">
        <h6 class="mt-5 fw-bold">What people say</h6>
        <h2 class="mb-5 fw-bold">Reviews</h2>
        <div class="row justify-content-around">
          <div class="col-3 round-photo">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi
              mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet
              placerat, ex nisi aliquam orci, ac varius odio libero et arcu.
            </p>
            <img
              src="../../public/images/avadabarbers-trimcut-gallery6-200x200.jpg"
              alt="John Doe"
            />
            <h6 class="text-capitalize fw-bold fst-italic">John Doe</h6>
          </div>
          <div class="col-3 round-photo">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi
              mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet
              placerat, ex nisi aliquam orci, ac varius odio libero et arcu.
            </p>
            <img
              src="../../public/images/avadabarbers-trimcut-gallery3-200x201.jpg"
              alt="Pete Jones"
            />
            <h6 class="text-capitalize fw-bold fst-italic">Pete Jones</h6>
          </div>
          <div class="col-3 round-photo">
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi
              mollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet
              placerat, ex nisi aliquam orci, ac varius odio libero et arcu.
            </p>
            <img
              src="../../public/images/avadabarbers-trimcut-gallery7-200x201.jpg"
              alt="Mark Wilson"
            />
            <h6 class="text-capitalize fw-bold fst-italic">Mark Wilson</h6>
          </div>
        </div>
      </div>
    </section>
    <!-- Blog posts -->
    <section id="blog" class="text-center pb-5">
      <div class="triangle-transiction"></div>
      <h6 class="mt-5 fw-bold">Tales from the barbershop</h6>
      <h2 class="mb-5 fw-bold">Recent Blog Posts</h2>
      <div class="container">
        <ul class="row justify-content-around">
          <li class="col-3">
            <img
              src="../../public/images/avadabarbers-second-blog-320x202.jpg"
              alt="second blog"
            />
            <div>
              <h4 class="mt-4 fw-bold">Avada Barbers Now Open</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Phasellus ut dapibus magna. Praesent semper,
              </p>
            </div>
          </li>
          <li class="col-3">
            <img
              src="../../public/images/avadabarbers-choosing-blog-320x202.jpg"
              alt="Choosing Blog"
            />
            <div>
              <h4 class="mt-4 fw-bold">Choosing The Right Barber</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Phasellus ut dapibus magna. Praesent semper,
              </p>
            </div>
          </li>
          <li class="col-3">
            <img
              src="../../public/images/avadabarbers-ourservice-blog-320x202.jpg"
              alt="ourservices"
            />
            <div>
              <h4 class="mt-4 fw-bold">Quick Service Guide</h4>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Phasellus ut dapibus magna. Praesent semper,
              </p>
            </div>
          </li>
        </ul>
      </div>
      <button class="mb-5 goldenrod_btn btn-general">
        Read more from our blog
      </button>
    </section>
    <!-- Blog posts -->
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
  text-transform: uppercase;
  font-weight: 700;
}

h4 {
  font-size: 32px;
  color: $driftWood;
}

h6 {
  color: $driftWood;
  font-size: 14px;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-weight: 600;
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
        $codGray 0
      ),
      linear-gradient(to top right, $codGray 50%, transparent 0);
  }
}
// SECTION PRODUCTS

#products {
  background: url(../../public/images/avadabarbers-reviewsbackground.jpg) top
    center;

  img {
    height: 50%;
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
    background: url(../../public/images/avadabarbers-cta-background.jpg);
  }

  h2 {
    color: $silverChalice;
  }
  .row {
    .round-photo {
      img {
        border-radius: 50%;
        height: 120px;
        width: 120px;
        margin: 15px 0;
      }
    }
  }
  // SECTION BLOG

  #blog {
    background: $ebb;
    .triangle-transiction {
      background-image: linear-gradient(to top right, transparent 50%, $white 0),
        linear-gradient(to bottom right, $white 50%, transparent 0);
    }
  }
}
</style>