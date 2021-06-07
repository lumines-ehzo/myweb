<template>
  <b-container class="content">
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
  </b-container>
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

<style scoped>
body {
  color: white;
}
.content {
  display: flex;
  padding-left: 10px;
  padding-top: 10px;
}

</style>