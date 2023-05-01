<template>
  <div class="about mx-1">
    <v-row class="container">

      <v-col cols="6" class="container__text">
        <div class="pa-5 py-1 font-size">
          <h1>About Company</h1>
          <strong>
            QAWS AlMatar International Company

          </strong>
        </div>
        <br />
        <br />
        <br />
        <div class="pa-5 py-1 font-size">
          <div><span class="color">Phone: </span><a style="color:black" href="tel:+971-4-3484858"> 971-4-3484858</a>
          </div>&nbsp;
          <div><span class="color">Whatsapp: </span><a style="color:black" href="tel:+971-52-6169172"> 971 52 616 9172</a>
          </div>&nbsp;
          <div><span class="color">Location: </span> Deira ,baniyas st, twin towers 22d floor, inox bussines center ,unit
            no:9
          </div>&nbsp;
          <div><span class="color">Mail: </span><a style="color:black" href = "mailto: info@qaws-al-matar.com">info@qaws-al-matar.com</a></div>
        </div>


      </v-col>
      <v-col cols="6" class="container__map">
        <div class="google-map mx-5 pa-5 px-1">
          <div class="mapouter">
            <div class="gmap_canvas"><iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3608.138154200142!2d55.3089024!3d25.265937599999997!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3e5f433661ee2cfb%3A0x41cafba46e7b8d75!2sDeira%20Twin%20Towers!5e0!3m2!1sen!2s!4v1682610448273!5m2!1sen!2s"
                class="container__mapSize" style="border:0;" loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"></iframe><a href="https://getasearch.com/fmovies"></a><br>
            </div>
          </div>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/mixin';
.gmap_canvas {
  overflow: hidden;
  background: none !important;
  height: 500px;
  width: 100%;
}

.mapouter {
  position: relative;
  text-align: right;
  height: 500px;
  width: 100%;
}
.font-size{
  @include responsive-font-size(12px);
}
.color {
  color: chocolate;
}

.container {
  // border: 3px solid blue;

  // max-width: 640px;
  &__map {
    display: inline-block;
    vertical-align: top;
    width: 46%;

  }

  &__mapSize {

    width: 100%;
    height: 500px;

    @media (max-width: 620px) {
      width: 100%;
      height: 250px;
    }
  }

  &__text {
    display: inline-block;
    width: 46%;
    overflow-y: auto;

  }
}

</style>
