<template>
  <div class="container text-center">
    <h6 class="mt-5 fw-bold">What people say</h6>
    <h2 class="mb-5 fw-bold">Reviews</h2>
    <div class="row justify-content-around">
      <div li v-for="(people, i) in reviews" :key="i" class="col-3 round-photo">
        <p>
          {{ people.description }}
        </p>
        <img
          :src="require(`../../public/images/${people.url}`)"
          alt="John Doe"
        />
        <h6 class="text-capitalize fw-bold fst-italic">
          {{ people.title }}
        </h6>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionReview",
  data() {
    return {
      reviews: [
        {
          title: "John Doe",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbimollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet placerat, ex nisi aliquam orci, ac varius odio libero et arcu.",
          url: "avadabarbers-trimcut-gallery6-200x200.jpg",
        },
        {
          title: "Pete Jones",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbimollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet placerat, ex nisi aliquam orci, ac varius odio libero et arcu.",
          url: "avadabarbers-trimcut-gallery3-200x201.jpg",
        },
        {
          title: "Mark Wilson",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbimollis eleifend ante ut sagittis. Sed sodales, urna et imperdiet placerat, ex nisi aliquam orci, ac varius odio libero et arcu.",
          url: "avadabarbers-trimcut-gallery7-200x201.jpg",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/sass/style.scss";

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
</style>