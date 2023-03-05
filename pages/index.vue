<template>
  <div>
    <div class="maxWidht container-fluid d-flex flex-column align-items-center">
      <!-- Muka + text desktop -->
      <div class="d-flex flex-column-reverse flex-lg-row align-items-center">
        <div class="bg-danger d-flex flex-column justify-content-center container-fluid" style="max-width: 700px;">
          <div class="bg-success pr-5 h-auto">
            <h1><strong>
              Timeless insights for business and life.
            </strong></h1>
            <h4>
              Every week, I sit down with someone in the Top 1% of their field
               — from NYT bestselling authors to Oscar winners — to decode 
               what they've mastered. Listen as I uncover the tactics, 
               routines, and habits that will propel you to the top of your field.
            </h4>
          </div>
          <div class="bg-primary d-flex flex-column m-2 align-items-center">
              <div class="bg-success" style="width: 200px;">
                s
              </div>
              <div class="d-flex">
                <div class="start bg-danger">
                  k
                </div>
                <div class="bg-dark">
                  u
                </div>           
              </div>
          </div>
        </div>
        <div class="bg-secondary w-50">
          <b-img src="~assets/images/5f479acca51c91168e689008_card-portrait-tiny.png" alt=""
           fluid></b-img>
        </div>
      </div>
      <!-- sponsor? desktop -->
      <div class="d-flex">
        <div class="fll">
          espn
        </div>
        <div class="flfl">
          washing
        </div>
      </div>
      <!-- slider element desktop -->
      <vueper-slides
        :visible-slides="3"
        slide-multiple
        :gap="3"
        :slide-ratio="1 / 4"
        :dragging-distance="200"
        :breakpoints="{ 800: { visibleSlides: 1, slideMultiple: 1 } }"
      >
      <vueper-slide
        v-for="i in 10"
        :key="i"
        :title="`title ${i}`"
        :image="`https://picsum.photos/id/${i}/400/300`"
      />
    </vueper-slides>
      <!-- interactive element desktop -->
      <div class="d-flex">
        <div class="">a</div>
        <div class="">b</div>
        <div class="">c</div>
      </div>
      <!-- now desktop -->
      <div class="now d-flex">
        <div class="">podc</div>
        <div class="">email</div>
      </div>
      <!-- email desktop -->
      <div class="text-center">
        Email
      </div>
    </div>
  </div>
</template>



<script>
  import { VueperSlides, VueperSlide } from "vueperslides";
  import "vueperslides/dist/vueperslides.css";
  
  export default {
    name: 'MyComponent',
    components: { 
      VueperSlides, 
      VueperSlide
    },
    layout: 'default',
  }
  
</script>

<style>
 .maxWidht{
    max-width: 1400px;
    padding-left: 30px;
    padding-right: 30px;
 }
</style>