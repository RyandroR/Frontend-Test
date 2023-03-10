<template>
  <div>
    <div class="container-fluid d-flex flex-column align-items-center">
      <!-- Muka + text -->
      <div class="w-100 d-flex justify-content-center" style="background-color: #050505;">
        <div class="maxWidht d-flex flex-column-reverse flex-lg-row align-items-center text-white">
          <div class="d-flex flex-column justify-content-center align-items-center align-items-lg-start container-fluid" style="max-width: 700px;">
            <div class="pr-lg-5 text-center text-lg-left w-75">
              <h2><strong class="font-weight-bold">
                Timeless insights for business and life.
              </strong></h2>
              <p class="h5" style="line-height: 30px;">
                Every week, I sit down with someone in the Top 1% of their field
                 — from NYT bestselling authors to Oscar winners — to decode 
                 what they've mastered. Listen as I uncover the tactics, 
                 routines, and habits that will propel you to the top of your field.
              </p>
            </div>
            <div class="d-flex flex-column m-2 align-items-center" style="max-width: 388px">
                <div class="d-flex align-items-center p-2 rounded-border bg-color-dark-grey">
                  <b-img src="~/assets/images/6377a5afa34a16823a370420_Ezra_Outlier-Founders_Episode-Card.jpg"
                  style="width: 100px; height: 80px; object-fit: cover;">
                  </b-img>
                  <div class="container">
                    <div class="text-warning">
                      <strong>
                        LATEST EPISODE
                      </strong> 
                    </div>
                    <div style="font-size: 14px;">
                      <strong>
                        #146 Ezra: Bringing Fast and Affordable Early Cancer Detection to Everyone | Emi Gal, Founder & CEO
                      </strong>
                    </div>  
                  </div>
                </div>
                <div class="d-flex justify-content-between w-100 mt-1">
                  <div class=" pr-4 pl-4 pt-2 pb-2 rounded-border bg-color-dark-grey" >
                    <h5 style="margin: 0;">Start Here</h5>
                  </div>
                  <div class=" pr-4 pl-4 pt-2 pb-2 rounded-border bg-color-dark-grey">
                    <h5 style="margin: 0;">Listen to the Podcast</h5>
                  </div>           
                </div>
            </div>
          </div>
          <div class="w-50">
            <b-img src="~assets/images/5f479acca51c91168e689008_card-portrait-tiny.png" alt=""
             fluid></b-img>
          </div>
        </div>
      
      </div>
      <!-- sponsor -->
      
      <div class="w-100 bg-color-dark-grey d-flex justify-content-center" style="border-top: 2px solid; border-bottom: 2px solid; border-color: #333333;">
        <div class="d-flex ">
          <div class="d-flex">
            <b-img src="~assets/images/billboard.svg" fluid></b-img>
          </div>
          <div class="d-flex">
            <b-img src="~assets/images/nytimes.svg" fluid></b-img>
          </div>
          <div class="d-flex">
            <b-img src="~assets/images/bloomberg.svg" fluid></b-img>
          </div>
          <div class="d-flex">
            <b-img src="~assets/images/washpost.svg" fluid></b-img>
          </div>
          <div class="d-flex">
            <b-img src="~assets/images/espn.svg" fluid></b-img>
          </div>
        </div>
      </div>
      <!-- slider element -->
      <div class="w-100 bg-color-dark-grey d-flex justify-content-center">
        <div class="slider w-100 container-fluid bg-color-dark-grey maxWidht" style="margin-top: 50px;">
          <vueper-slides
            :visible-slides="3"
            slide-multiple
            :gap="3"
            :slide-ratio="1/3"
            :dragging-distance="200"
            :breakpoints="{ 900: { visibleSlides: 1, slideMultiple: 1 } }"
            class="no-shadow"
            
            fixed-height= "700px"
          >
          <vueper-slide
            v-for="i in 9"
            :key="i"
            :title="`title ${i}`"
            :image="`https://upload.wikimedia.org/wikipedia/commons/5/59/Empty.png`"
          >
            <template #content>
              <div slot="slideCon" class=" d-flex flex-column h-100 bg-white" 
              style="border-radius: 16px;">
                <b-img src="~/assets/images/6377a5afa34a16823a370420_Ezra_Outlier-Founders_Episode-Card.jpg"
                style="width: 280; height: 280px; object-fit: cover; border-top-left-radius: 16px; border-top-right-radius: 16px;"></b-img>
                <div class="p-3">
                  <strong>#146 Ezra: Bringing Fast and Affordable Early Cancer Detection to Everyone | Emi Gal, Founder & CEO </strong>
                  Learn how to unlock your originality and awaken your creative genius as we break down The Laws of Creativity by Joey Cofone, award-winning designer and Founder & CEO of the much loved “Tools for Thinkers” brand Baronfig.
                </div>
              </div>
            </template>
          </vueper-slide>
          
          </vueper-slides>
        </div>

      </div>
      <!-- interactive element -->
      <div class="w-100 d-flex justify-content-center bg-color-dark-grey flex-column flex-lg-row align-items-center">
        <div class="d-flex container-fluid row flex-column flex-lg-row align-items-center justify-content-center maxWidht" style="margin-top: 25px;">
          <div class="bg-white col text-center hoverthis hover_element d-flex flex-column align-items-center justify-content-center border-rounded-no-color" 
          style="padding-left: 50px; padding-right: 50px; padding-top: 25px; padding-bottom: 25px;">
            <div class="rounded-circle hoverable-background d-flex justify-content-center align-items-center" style="height: 75px; width: 75px;">
              <b-img src="~assets/images/popular.svg" class="" ></b-img>
            </div>
            <div class="hoverable-text">
              <strong>
                TRENDING NOW
              </strong>
            </div>
            <div class="hoverable-text">
              <strong>
                Find the interview and articles that are trending now
              </strong>
            </div>
          </div>
          <div class="bg-white p-4 col text-center hoverthis hover_element d-flex flex-column align-items-center justify-content-center border-rounded-no-color"
          style="padding-left: 50px; padding-right: 50px; padding-top: 25px; padding-bottom: 25px;">
            <div class=" rounded-circle hoverable-background d-flex justify-content-center align-items-center" style="height: 75px; width: 75px;">
              <b-img src="~assets/images/latestposts.svg" class=""></b-img>
            </div>
            <div class="hoverable-text">
              <strong>
                NEW RELEASE 
              </strong>
            </div>
            <div class="hoverable-text">
              <strong>
                Catch up on all of the latest interviews and articles
              </strong>
            </div>
          </div>
          <div class="bg-white p-4 col text-center hoverthis d-flex flex-column align-items-center justify-content-center border-rounded-no-color"
          style="padding-left: 50px; padding-right: 50px; padding-top: 25px; padding-bottom: 25px;">
            <div class="rounded-circle hoverable-background d-flex justify-content-center align-items-center" style="height: 75px; width: 75px;">
              <b-img src="~assets/images/topicsandtags.svg" class=""></b-img>
            </div>
            <div class="hoverable-text">
              <strong>
                ARCHIVE
              </strong>
            </div>
            <div class="hoverable-text">
              <strong>
                Explore the archives by browsing categories and tags
              </strong>
            </div>
          </div>
        </div>
      </div>
      <!-- outliers -->
      <div class="w-100 bg-color-dark-grey d-flex justify-content-center">
        <div class="now d-flex flex-column-reverse flex-lg-row align-items-center maxWidht justify-content-between ">
          <div class="mt-4" style="width: 48.5%;">
            <div class="rounded-border container-fluid" style="max-width: 1400px; background-color: #333333;">
              <div class="text-center text-white">
                <div class="text-weight-bolder h3">LISTEN NOW</div>
                <div class="h2">Outliers Podcast</div>
                <div class="">Every week,I sit down with someone in the Top 1% of their</div>
                <div class="">field to decode what they've mastered and what they've </div>
                <div class="">learned along the way</div>
  
                <div class="">Explore Episodes</div>
              </div>
              <div class="d-flex">
                <div class="col">
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c1r1.jpg" fluid></b-img>
                  </div>
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c1r2.jpg" fluid></b-img>
                  </div>
                </div>
                <div class="col" >
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c2r1.jpg" fluid></b-img>
                  </div>
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c2r2.jpg" fluid></b-img>
                  </div>
                </div>
                <div class="col">
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c3r1.jpg" fluid></b-img>
                  </div>
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c3r2.jpg" fluid></b-img>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="mt-4" style="width: 48.5%;">
            <div class="rounded-border container-fluid" style="max-width: 1400px; background-color: #333333;">
              <div class="text-center text-white">
                <div class="text-weight-bolder h3">LISTEN NOW</div>
                <div class="h2">Friday 5 Email</div>
                <div class="">Every Friday, I share five things I've been reading, using,</div>
                <div class="">and loving—including articles, biohacks, gadgets, and</div>
                <div class="">more.</div>
                <div class="">Subscribe Now</div>
              </div>
              <div class="d-flex">
                <div class="col">
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c1r1f.jpg" fluid></b-img>
                  </div>
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c1r2f.jpg" fluid></b-img>
                  </div>
                </div>
                <div class="col" >
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c2r1f.jpg" fluid></b-img>
                  </div>
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c2r2f.jpg" fluid></b-img>
                  </div>
                </div>
                <div class="col">
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c3r1f.jpg" fluid></b-img>
                  </div>
                  <div class="row container-fluid margin-pad-0">
                    <b-img src="~/assets/images/c3r2f.jpg" fluid></b-img>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- email -->
      <div class="w-100 bg-color-dark-grey d-flex justify-content-center">
        <div class="text-center text-white pt-5 d-flex flex-column justify-content-center align-items-center"
        style="max-width: 560px;">
          <div class="">
            <div class="" 
            style= "font-weight: 1000 !important; font-size: 24px;">
              GET THE WEEKLY SUMMARY
            </div>
          </div>
          <div class="">
            Join 7,500+ including Fortune 500 CEOs, championship coaches, 
          </div>
          <div class="">
            and bestselling authors who get my free weekly summary.
          </div>
          <b-input-group class="w-75">
            <b-form-input placeholder="Enter your email..."></b-form-input>
            <b-input-group-append>
              <b-button variant="danger">Try It</b-button>
            </b-input-group-append>
          </b-input-group>
          <div class="text-muted">By subscribing, you agree to our privacy policy.</div>
        </div>
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
.rounded-border{
  border: 3px solid;
  border-radius: 15px;
  border-color: #333333;
}

.border-rounded-no-color{
  border: 1px solid;
  border-radius: 15px;
}

.bg-color-dark-grey{
  background-color: #222222;
}

.container-fluid{
  padding: 0;
}

.margin-pad-0{
  margin: 0;
  padding: 0;
}

 .maxWidht{
    max-width: 1400px;
    width: 100%;
    padding-left: 30px;
    padding-right: 30px;
 }

 .hover_element{
  margin-right: 3%;
}

  @media (max-width: 1199.98px) { 
    .hover_element{
      margin-right: 0;
      margin-bottom: 3%;
    } 
 }

 .podcast-friday-image{
  width: 31%;
 }

 .hoverable-text{
  color: black;
  transition: 1s;
 }
 .hoverable-background{
  background-color: black;
  transition: 1s;
 }

 .hoverthis:hover .hoverable-text{
  color: rgb(255,168,0);
 }

 .hoverthis:hover .hoverable-background{
  background-color: rgb(255,168,0);
 }
</style>
