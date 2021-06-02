<template>
  <div class="content">
    <div class="row">
      <div class="col-sm-8">
        <div class="media">
          <div class="media-body">
            <h5 class="mt-0">นาย รัฐภูมิ เรืองกล้า</h5>
            <p>
              นักศึกษา มจพ.คณะวิทยาศาสตร์ประยุกต์ ภาควิชาวิทยาการคอมพิวเตอร์(CS)
            </p>
            <p>
              ส่วนสูง 183 น้ำหนัก 55 เกิดวันจันทร์ ชอบสีน้ำเงิน ชอบทานข้าวผัด
            </p>
          </div>
        </div>
      </div>
      <div class="col-sm-8">
        <div>
          <b-carousel
            id="carousel-fade"
            style="text-shadow: 0px 0px 2px #000"
            fade
            indicators
            img-width="200"
            img-height="200"
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
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'navbar',
  data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
}
</script>

<style>
body {
  color: white;
}
.content {
  display: flex;
  padding-left: 10px;
  padding-top: 10px;
}
</style>