<template>
  <div>
    <div class="parallax-wrapper">
      <div class="hero parallax-content">
        <img
          src="~/assets/y3.jpg"
          alt="smart guy"
        />
        <div class="hero__title">
          <h1>My RESUME</h1>
          <p>
            Rattapoom Ruengkla
          </p>
        </div>
      </div>
      <div class="main-content">
        <h2>นาย รัฐภูมิ เรืองกล้า ชื่อเล่น ภูมิ</h2>
        <p>
          นักศึกษาฝึกงาน จากมหาวิทยาลัยเทคโนโลยีพระจอมเกล้าพระนครเหนือ
          อายุ 21 ปี เกิดวันจันทร์ที่ 21 กุมภาพันธ์ 2543 ราศี กุมภ์ สูง 183 หนัก 55
          สีที่ชอบ สีน้ำเงิน อาหารที่ชอบคือ ข้าวผัด งานอดิเรก ฟังเพลง,เล่นเกม,นอน,อ่านมังงะ
        </p>
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
          <h2>Education</h2>
        <p>
            King Mongkut's University of Technology<br>
            North Bangkok (KMUTNB)<br>
            in 2018 - Present<br>
            Department of Computer and Information Science,<br>
            Faculty of Applied Science<br>
            GPAX : 2.4<br>

            SAKAEO SCHOOL<br>
            Graduated in 2017<br>
            Science - Mathematics Program<br>
            GPAX : 3.4<br>

        </p>
        <h2>Project</h2>
        <p>
            - First-year Mini Project<br>
                "Vending Machine Simulator : Python"<br>
            - Sophomore Mini Project<br>
                "Helioz, Game Project OOP : JAVA"<br>
            - Sophomore Mini Project<br>
                "Claim System, Web-site : SQL,PHP"<br>
            - Junior Mini Project<br>
                "Book Store, Web-site : SQL,PHP"<br>
        </p>
        <h2>Contact</h2>
        <p>
          061-6831225<br>
          rattapoom.rue@gmail.com<br>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'navbar',
}
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;1,600&display=swap");

:root {
  --hero-gap: 60px;
}

* {
  box-sizing: border-box;
}
body {
  font-family: "Lora", serif;
}

h1 {
  font-size: calc(0.5rem + 8vmin);
  font-weight: 600;
  font-style: italic;
}

h2 {
  font-size: 30px;
  font-weight: 600;
  font-style: italic;
  line-height: 1.2;
}

p {
  font-size: 26px;
  line-height: 1.65;
}

.caption {
  position: absolute;
  bottom: 1rem;
  right: 1rem;
  color: white;
  z-index: 2;
  font-size: 0.6rem;
}

.parallax-wrapper {
  height: 100vh;
  overflow-x: hidden;
  overflow-y: scroll;
  perspective: 10px;
}

.parallax-content {
  position: relative;
  width: 100%;
  height: calc(100vh - var(--hero-gap));
}

.hero {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;

  img {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 120%;
    object-fit: cover;
    z-index: 1;
    transform: translateZ(1px);
  }

  .hero__title {
    color: white;
    z-index: 2;
    text-align: center;
    transform: translateZ(-2px) scale(1.2);

    p {
      margin-top: 0.5rem;
      font-size: calc(0.6rem + 0.75vmin);
    }

    a {
      color: white;
    }
  }

  &::after {
    content: "";
    position: absolute;
    top: 50%;
    left: 0;
    width: 100%;
    height: 100%;
    transform-origin: 0 100%;
    transform: translateZ(8px);
    pointer-events: none;
    background-image: linear-gradient(
      to bottom,
      hsla(0, 0%, 0%, 0) 0%,
      hsla(0, 0%, 0%, 0.013) 8%,
      hsla(0, 0%, 0%, 0.049) 14.8%,
      hsla(0, 0%, 0%, 0.104) 20.8%,
      hsla(0, 0%, 0%, 0.175) 26%,
      hsla(0, 0%, 0%, 0.259) 30.8%,
      hsla(0, 0%, 0%, 0.352) 35.3%,
      hsla(0, 0%, 0%, 0.45) 39.8%,
      hsla(0, 0%, 0%, 0.55) 44.5%,
      hsla(0, 0%, 0%, 0.648) 49.5%,
      hsla(0, 0%, 0%, 0.741) 55.2%,
      hsla(0, 0%, 0%, 0.825) 61.7%,
      hsla(0, 0%, 0%, 0.896) 69.2%,
      hsla(0, 0%, 0%, 0.951) 77.9%,
      hsla(0, 0%, 0%, 0.987) 88.1%,
      hsl(0, 0%, 0%) 100%
    );
    z-index: 3;
  }
}

.main-content {
  position: relative;
  margin: 0 auto;
  padding: var(--hero-gap) 2rem;
  max-width: 725px;
  background-color: white;

  > * + * {
    margin-top: 2rem;
  }
}


</style>
