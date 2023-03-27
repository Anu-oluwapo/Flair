<template>
  <section class="hero-section">
    <Line class="line" />
    <Line class="line2" />
    <div class="hero container">
      <div class="text">
        <h1>
          The Best<br />
          Platform To<br />
          DIscover Talents<br />
          & Models
        </h1>
        <p>
          At Flair, We identify amazing talents and models to help build an
          amazing industry and make hiring a lot easier
        </p>

        <button class="btn"><span>Discover</span></button>
      </div>

      <div class="images">
        <div
          @mouseover="scale('boy')"
          @mouseleave="scale('boy', true)"
          class="image"
        >
          <img src="/boy.png" id="boy" />
        </div>
        <div
          @mouseover="scale('girl')"
          @mouseleave="scale('girl', true)"
          class="image"
        >
          <img id="girl" src="/girl.png" />
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Line from "@/components/icons/Line.vue";
import { gsap } from "gsap";
import { onMounted } from "vue";

function scale(id, reverse) {
  let tl = gsap.timeline();
  tl.to(`#${id}`, {
    transform: "scale(120%)",
  });

  if (reverse) {
    tl.to(
      `#${id}`,
      {
        transform: "scale(100%)",
      },
      0
    );
  }
}

onMounted(() => {
  let tl = gsap.timeline();

  tl.fromTo(
    ".image",
    { height: 0 },
    { duration: 1.5, stagger: 0.2, height: "auto", ease: "Power4.easeInOut" },
    1
  ).from(
    "img",
    {
      duration: 1.5,
      stagger: 0.2,
      transform: "scale(200%)",
      ease: "Power4.easeInOut",
    },
    1
  );
});
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";
.line {
  position: absolute;
  top: 0;
  z-index: -1;
}
.line2 {
  position: absolute;
  top: 0;
  right: 0;
  transform: scaleX(-1);
  z-index: -1;
}

.images {
  display: flex;
  width: 100%;
  position: relative;
  height: 100%;
  .image {
    background: $gray;
    position: absolute;
    width: 50%;
    overflow: hidden;
    height: auto;
    &:nth-child(2) {
      background: $gray2;
      top: 10rem;
      right: 5rem;
    }
    img {
      width: 100%;
      display: block;
      margin: 0 auto;
      //   transition: all 3s ease;
      // margin-left: ;
    }

    &:hover {
      img {
        transform: scale(120%);
      }
    }
  }
}
</style>
