<template>
  <section class="about-section">
    <Line class="line" />
    <Line class="line2" />
    <div class="about">
      <div class="container">
        <img id="" src="/about.png" />

        <div class="text">
          <h1>What We Do</h1>
          <p>
            FLAIR.ng is a modern modelling and talent agency which scouts for
            and identifies incredible and amazing models and talents. We provide
            our clients with te best talents out there to help build and boost
            their brands or companies.
          </p>

          <button class="btn"><span>Discover</span></button>
        </div>
      </div>

      <div class="container">
        <img id="" src="/about2.png" />

        <div class="text">
          <h1>Hiring Made Easy</h1>
          <p>
            FLAIR.ng is a modern modelling and talent agency which scouts for
            and identifies incredible and amazing models and talents. We provide
            our clients with te best talents out there to help build and boost
            their brands or companies.
          </p>

          <button class="btn"><span>Hire Now</span></button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// import Line from "@/components/icons/Line.vue";
// import { gsap } from "gsap";
// import { onMounted } from "vue";

// function scale(id, reverse) {
//   let tl = gsap.timeline();
//   tl.to(`#${id}`, {
//     transform: "scale(110%)",
//   });

//   if (reverse) {
//     tl.to(
//       `#${id}`,
//       {
//         transform: "scale(100%)",
//       },
//       0
//     );
//   }
// }

// onMounted(() => {
//   let tl = gsap.timeline();

//   tl.fromTo(
//     ".image",
//     { height: 0 },
//     { duration: 1.5, stagger: 0.2, height: "auto", ease: "Power4.easeInOut" },
//     1
//   ).from(
//     "img",
//     {
//       duration: 1.5,
//       stagger: 0.2,
//       transform: "scale(200%)",
//       ease: "Power4.easeInOut",
//     },
//     1
//   );
// });
</script>

<style lang="scss" scoped></style>
