<template>
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
    <div class="container" id="section-3">
      <h6 class="text-uppercase fw-bold mt-5 text-center">
        We have you covered
      </h6>
      <h2 class="mb-5 fw-bold text-center">Avada Grooming Products</h2>
      <ul class="row maxh-400">
        <li v-for="(shop, i) in products" :key="i" class="col-3">
          <img
            :src="require(`../../public/images/${shop.url}`)"
            alt="Dark brush"
          />
          <h4 class="fw-bold">{{ shop.title }}</h4>
          <p class="text-gold"><span class="fs-4">$</span>{{ shop.price }}</p>
        </li>
      </ul>
    </div>
    <button class="mb-5 goldenrod_btn btn-general">
      Shop our product range
    </button>
  </section>
  <!-- CLOSE SECTION PRODUCTS -->
</template>

<script>
export default {
  name: "SectionProduct",
  data() {
    return {
      // DATI SEZIONE SHOP
      products: [
        {
          title: "Brush",
          price: "15.00",
          url: "brush_dark-400x400.png",
        },
        {
          title: "Scissor",
          price: "85.00",
          url: "scissors-400x400.png",
        },
        {
          title: "Beard Tidy",
          price: "15.00",
          url: "hot_oil_dark-400x400.png",
        },
        {
          title: "Straight Razor",
          price: "30.00",
          url: "straight_razor_dark-400x400.png",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

#products {
  background: $bgProdutcts top center;

  img {
    height: 50%;
  }
  h2 {
    font-size: 50px;
  }
}
</style>