<template>
  <section id="blog" class="text-center pb-5">
    <div class="triangle-transiction" id="section-5"></div>
    <h6 class="mt-5 fw-bold">Tales from the barbershop</h6>
    <h2 class="mb-5 fw-bold">Recent Blog Posts</h2>
    <div class="container">
      <ul class="row justify-content-around">
        <li v-for="(article, i) in blogs" :key="i" class="col-3">
          <img
            :src="require(`../../public/images/${article.url}`)"
            alt="second blog"
          />
          <div>
            <h4 class="mt-4 fw-bold">{{ article.title }}</h4>
            <p>
              {{ article.description }}
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
</template>

<script>
export default {
  name: "SectionBlog",
  data() {
    return {
      // DATI SEZIONE SHOP
      blogs: [
        {
          title: "Avada Barbers Now Open",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut dapibus magna. Praesent semper,",
          url: "avadabarbers-second-blog-320x202.jpg",
        },
        {
          title: "Choosing The Right Barber",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut dapibus magna. Praesent semper,",
          url: "avadabarbers-choosing-blog-320x202.jpg",
        },
        {
          title: "Quick Service Guide",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut dapibus magna. Praesent semper,",
          url: "avadabarbers-ourservice-blog-320x202.jpg",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

// SECTION BLOG

#blog {
  background: $ebb;
  .triangle-transiction {
    background-image: linear-gradient(to top right, transparent 50%, $white 0),
      linear-gradient(to bottom right, $white 50%, transparent 0);
  }
  h2 {
    color: $silverChalice;
  }
  h4 {
    font-size: 30px;
  }
  h6 {
    font-size: 14px;
  }
}
</style>