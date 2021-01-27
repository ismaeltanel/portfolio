<!-- pages/index.vue -->

<template>
  <div>
    <section id="hpage">
      <img id="moonC" class="moonCircle" src="../assets/mcbig2.svg" />

      <div>
        <img class="moonDot" src="../assets/moondot.png" />
        <div class="verticalFade"></div>
      </div>

      <div>
        <img class="moonDotR" src="../assets/moondot.png" />
        <div class="verticalFadeR"></div>
      </div>

      <a href="#about"
        ><img class="geoCardA" src="../assets/aboutNoText3.svg"
      /></a>
      <a href="#works"
        ><img class="geoCardW" src="../assets/aboutNoText3.svg"
      /></a>
      <a href="#contact"
        ><img class="geoCardC" src="../assets/aboutNoText3.svg"
      /></a>
    </section>

    <section id="about">
      <div class="diamondU">
        <svg>
          <defs>
            <linearGradient id="myGradient">
              <stop offset="5%" stop-color="#cee9fa" />
              <stop offset="45%" stop-color="transparent" />
            </linearGradient>
          </defs>
          <defs>
            <linearGradient id="myGradient2">
              <stop offset="5%" stop-color="transparent" />
              <stop offset="85%" stop-color="#cee9fa" />
            </linearGradient>
          </defs>
          <rect
            x="171"
            y="70"
            width="310"
            height="1"
            fill="url('#myGradient')"
          />
          <rect
            x="10"
            y="70"
            width="141"
            height="1"
            fill="url('#myGradient2')"
          />
          <svg>
            <g>
              <polygon
                fill="#8752de"
                points="116.008,115 125,96.909 133.992,115 
		125,123.092 "
                transform="scale(1) translate(36, -44)"
              />
            </g>
          </svg>
        </svg>
      </div>
      <div>
        <h1 class="line1">Surprise motherfucker </h1>
      </div>

      <div>
        <h1 class="line2">It's me, Tanel Ismael.</h1>
      </div>

      <div>
        <h1 class="line3">From Estonia</h1>
      </div>

      <div>
        <h1 class="line4">27 years of age.</h1>
      </div>

      <div>
        <h1 class="line5">I enjoy UI/UX Web Dev Game Dev</h1>
      </div>

      <div>
        <h1>CV button</h1>
      </div>
      <hr>
    </section>

    <section id="works">
      <!--<img class="worksSelect" src="~/assets/IngameDesign.png" />-->
      <div v-swiper="swiperOption">
        <div class="swiper-wrapper">
          <div class="swiper-slide">
            <nuxt-link to="/works/test"
              ><img src="1.jpg" alt="" />
              <p class="interfaceP">Interface Design</p>
              <div class="svg-wrapper">
                <svg height="60" width="320" xmlns="http://www.w3.org/2000/svg">
                  <rect class="shape" height="60" width="320" />
                </svg></div
            ></nuxt-link>
          </div>
          <div class="swiper-slide">
            <img src="2.jpg" alt="" />
          </div>
          <div class="swiper-slide">
            <img src="3.jpg" alt="" />
          </div>
          <div class="swiper-slide">
            <img src="5.jpg" alt="" />
          </div>
          <div class="swiper-pagination swiper-pagination-bullets"></div>
        </div>
      </div>
    </section>

    <section class="section is-large" id="contact">
      <hr />

      <p>Tanel Ismael 2021 &copy;</p>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      swiperOption: {
        loop: true,
        centeredSlides: true,
        slidesPerView: "auto",
        spaceBetween: 210,
        pagination: {
          el: ".swiper-pagination",
          dynamicBullets: true,
        },
      },
    };
  },
};
</script>


<style scoped>
#hpage {
  background-color: #0e0f24;
  background: url(../assets/BG1.png);
  background-repeat: no-repeat;
  background-attachment: scroll;
  background-size: cover;
  background-position: center center;
  min-height: 100vh;
  max-width: 100vw;
  margin: 0 auto;
}

.moonCircle {
  position: absolute;
  left: 30vw;
  top: 15vh;
  width: 40%;
}

.geoCardA {
  position: absolute;
  left: 20vw;
  top: 24vh;
  width: 50%;
  max-width: 13%;
}

.geoCardW {
  position: absolute;
  left: 43.3vw;
  top: 24vh;
  width: 50%;
  max-width: 13%;
  margin: auto;
  display: block;
}

.geoCardC {
  position: absolute;
  right: 20vw;
  top: 24vh;
  width: 50%;
  max-width: 13%;
}

.verticalFade {
  position: absolute;
  left: 10vw;
  top: 28vh;
  width: 1px;
  height: 350px;
  border: 2px solid;
  border-top: 0;
  border-bottom: 0;
  border-right: 0;
  border-image: linear-gradient(
    to bottom,
    rgba(255, 255, 255, 0) 0%,
    rgba(101, 111, 133, 0.664) 50%,
    rgba(255, 255, 255, 0) 100%
  );
  border-image-slice: 1;
}

.verticalFadeR {
  position: absolute;
  right: 10vw;
  top: 28vh;
  width: 1px;
  height: 350px;
  border: 2px solid;
  border-top: 0;
  border-bottom: 0;
  border-left: 0;
  border-image: linear-gradient(
    to bottom,
    rgba(255, 255, 255, 0) 0%,
    rgba(101, 111, 133, 0.664) 50%,
    rgba(255, 255, 255, 0) 100%
  );
  border-image-slice: 1;
}

.moonDot {
  position: absolute;
  left: 6.5vw;
  top: 45vh;
}

.moonDotR {
  position: absolute;
  right: 6.5vw;
  top: 45vh;
  transform: scaleX(-1);
}

#about {
  background-color: #0e0f24;
  min-height: 100vh;
  max-width: 100vw;
  margin: 0 auto;
}

#about h1 {
  font-size: 40px;
  padding-bottom:30px;
  text-align: center;
}

.line1 {
  padding-right: 500px;
}

.line2 {
  padding-left: 500px;
}

.line3 {
  padding-right: 500px;
}

.line4 {
   padding-left: 500px;
}

.line5 {
  padding-right: 300px;
}


.diamondU {
  display: flex;
  justify-content: center;
  align-items: center;
}

hr {
  margin:auto;
  margin-top: 50px ;
  width: 50%;
}

#works {
  background-color: #0e0f24;
  position: relative;
  min-height: 100vh;
  max-width: 100vw;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

.worksSelect {
  width: 50%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
  width: 50%;
}

:hover.swiper-slide-active {
  filter: brightness(50%);
  z-index: 2;
}
:hover.swiper-slide-active p {
  font-size: 50px;
  filter: brightness(100%);
  position: absolute;
  text-align: center;
  z-index: 222;
  color: white;
  left: 0;
  right: 0;
  top: 17vh;
  margin-left: auto;
  margin-right: auto;
  display: block;
}

.interfaceP {
  display: none;
}

.swiper-slide-next {
  filter: brightness(30%);
}

.swiper-slide-prev {
  filter: brightness(30%);
}

.swiper-slide:nth-child(2n) {
  width: 50%;
}

.swiper-slide:nth-child(3n) {
  width: 50%;
}

.svg-wrapper {
  position: absolute;
  top: 35%;
  transform: translateY(-65%);
  margin: 0 auto;
  width: 320px;
  left: 50%;
  transform: translateX(-50%);
}
.shape {
  stroke-dasharray: 140 540;
  stroke-dashoffset: -474;
  stroke-width: 8px;
  fill: transparent;
  stroke: #ffffff;
  border-bottom: 5px solid black;
  transition: stroke-width 1s, stroke-dashoffset 1s, stroke-dasharray 1s;
}
.text {
  font-family: "Roboto Condensed";
  font-size: 22px;
  line-height: 32px;
  letter-spacing: 8px;
  color: #fff;
  top: -48px;
  position: relative;
}
.svg-wrapper:hover .shape {
  stroke-width: 2px;
  stroke-dashoffset: 0;
  stroke-dasharray: 760;
}

#contact {
  background-color: #0e0f24;
  min-height: 100vh;
  max-width: 100vw;
  margin: 0 auto;
}
</style>





