<template>
  <!-- <b-container class="content">
    <b-row>
      <b-col>
        <h6>RESUME</h6>
        <h5>RATTAPOOM RUENGKLA</h5>

        <div>
          <b-carousel
            id="carousel-fade"
            style="text-shadow: 0px 0px 2px #000"
            fade
            indicators
            img-width="1280"
            img-height="720"
          >
            <b-carousel-slide
              caption="ปี 1"
              img-src="~/assets/y1.jpg"
            ></b-carousel-slide>
            <b-carousel-slide
              caption="ปี 2"
              img-src="~/assets/y2.2.jpg"
            ></b-carousel-slide>
            <b-carousel-slide
              caption="ปี 3"
              img-src="~/assets/y3.jpg"
            ></b-carousel-slide>
          </b-carousel>
        </div>
      </b-col>
    </b-row>
  </b-container> -->
  <div>
    <div class="parallax-wrapper">
      <div class="hero parallax-content">
        <img src="~/assets/y3.jpg" alt="smart guy" />
        <div class="hero__title">
          <h1>Welcome!</h1>
        </div>
      </div>
      <!-- <section class="text" style="--bg: #c8c8bc">
        <h1>Armenian highlands</h1>
      </section> -->
      <div class="hero parallax-content">
        <img src="~/assets/y2.2.jpg" alt="smart guy" />
        <div class="hero__title">
          <h1>To My Website!</h1>
        </div>
      </div>
      <!-- <section class="text" style="--bg: #638a87">
        <h1>Paradise on earth</h1>
      </section> -->
      <div class="hero parallax-content">
        <img src="~/assets/y1.jpg" alt="smart guy" />
        <div class="hero__title">
          <h1>Test!</h1>
        </div>
      </div>
      <!-- <section class="text" style="--bg: #384558">
        <h1>Far, far away...</h1>
      </section> -->
    </div>
  </div>
</template>

<script>
export default {
  layout: 'navbar',
  data() {
    return {
      slide: 0,
      sliding: null,
    }
  },
  methods: {
    onSlideStart(slide) {
      this.sliding = true
    },
    onSlideEnd(slide) {
      this.sliding = false
    },
  },
}
</script>

<style lang="scss">
// html,
// body {
//   background-color: black;
// }
// .container {
//   height: 100vh;
//   overflow-x: hidden;
//   overflow-y: scroll;
//   perspective: 10px;
// }

// section {
//   position: relative;
//   display: flex;
//   align-items: center;
//   justify-content: center;
//   overflow: hidden;
//   &.image {
//     background-position: center center;
//     transform: translateZ(-1px) scale(1.5);
//     /* Force the background image to fill the whole element. */
//     background-size: cover;
//     /* Keep the image from overlapping sibling elements. */
//     z-index: -1;
//     height: 100vh;
//   }
//   &.text {
//     height: 50vh;
//   }
//   &.heading {
//     z-index: -1;
//     transform: translateY(-30vh) translateZ(1px) scale(1.5);
//   }
// }

// .footer {
//   position: relative;
//   display: block;
//   background-color: black;
//   height: 100vh;
//   color: white;
//   display: flex;
//   align-items: center;
//   justify-content: center;
//   h3 {
//     font-weight: normal;
//     color: var(--color-blue);
//   }
// }
</style>