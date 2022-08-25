<template>
  <section id="services">
    <div class="container" id="section-2">
      <h6 class="text-uppercase mt-5 fw-bold text-center">Men's grooming</h6>
      <h2 class="fw-bold text-center">Services</h2>

      <ul class="row text-center py-5 justify-content-around">
        <!-- LOGICA PER GIRARE Nell'OGG. Services -->
        <li v-for="(service, i) in services" :key="i" class="col-3 mt-4">
          <img
            :src="require(`../../public/images/${service.url}`)"
            alt="Men's Grooming"
          />
          <h4 class="py-5 fw-bold">{{ service.title }}</h4>
          <p>
            {{ service.description }}
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
</template>

<script>
export default {
  name: " SectionServices",
  data() {
    return {
      services: [
        {
          title: "Trim & Cut",
          description:
            "Avada Barbers are experts in the lickety split trim and hair cut. Quick but careful and ridiculously good looking.",
          url: "avadabarbers-trimcut-icon-before.png",
        },
        {
          title: "Wash & Dry",
          description:
            "Take a seat in our fine leather chairs, lean back and let us lather you a fresh head in a luxurious fashion.",
          url: "avadabarbers-washndry-icon.png",
        },
        {
          title: "Quick Service Guide",
          description:
            "Tame the tangles and untidy facial hairs like a gentleman with our Beard Tidy services from Avada Barbers.",
          url: "avadabarbers-beardtrim-icon.png",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

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
</style>