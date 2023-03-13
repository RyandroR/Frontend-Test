<template>
    <div>
        <AppHeader v-if="!handleView()" />

        <div class="w-100" v-if="handleView()"
        style="background-color: #333333;">
            <div class="d-flex justify-content-between">
                <b-button v-b-toggle.collapse-1 variant="secondary">
                    Burger Icon
                </b-button>
                <svg xmlns="http://www.w3.org/2000/svg" 
                style="width: 175px; fill: white;" id="Layer_1" width="100%" height="100%" data-name="Layer 1" viewBox="0 0 1479.9 180"><defs></defs><path d="M1074.9 72.8a13 13 0 0 0 10.9-3.8c4.5-4.4 3-11.3-2.9-13.6a24.4 24.4 0 0 0-6.6-1.5 9.2 9.2 0 0 0-10.3 7.9 1.7 1.7 0 0 0-.1.7c-.4 5.3 3.4 9.7 9 10.3ZM537 75.6a12.8 12.8 0 0 0 11.1-3.9 8 8 0 0 0 .3-11.3 7.5 7.5 0 0 0-3-2 27.1 27.1 0 0 0-6.8-1.7 9.2 9.2 0 0 0-10.4 8 1.3 1.3 0 0 0-.1.6 9.6 9.6 0 0 0 8.8 10.3ZM292.4 67.9C291.1 21 244.4.7 205.4.1 147.5-.7 14.2 31.1.8 86.4-10.1 131 97.3 149.6 128.4 160c17.6 5.8 18.6 13.6 20.8 16.4 4.4 5.3 11.4 4.7 14.4-1.5a25.3 25.3 0 0 0 2.2-7.7 237.1 237.1 0 0 1 11.3-44.6c11.2-31.5 13.7-38 14.1-49.5s-14.5-15.8-20.2-4.5c-8 15.9-1.9 21.4-4.3 30-4.5 15.8-9.2 31.6-13.8 47.4-.9 3-2.1 3.2-5.1 1.8-45.6-21.1-138.3-34.6-126.6-61.2 17.7-40.2 137.7-70.8 184.4-68.8s69.7 25.9 69 53.5c-1.1 50.8-69.6 70-85 75.1-8.5 2.8-7.1 18.4 9.6 16.9 6-.5 35.9-12.6 64-34.8 19.8-15.5 29.9-35.7 29.2-60.6ZM1470.2 71.3c-6-5.2-15.6.7-13.2 8.7 1.3 4.5 4.6 7.1 6.1 8.7 3 3.1 3.2 5 .6 8.5-11.6 16.2-39.9 31.6-57.4 26.7-5-1.4-7.7-4.4-8.2-9.5-.2-2.5-.2-5-.2-7.5.2-13.3-6.4-22.2-18.3-27.6-14.8-6.8-33.8-8.6-41.4-6.6s-10.4 9.6-6.5 16 12.9 9.4 4.8 19.1-16.3 12.4-27 13.2a41.2 41.2 0 0 1-12.1-1.2c-3.4-.8-3.6-2.8-1.1-5.2s10.8-9 15.1-20.5-10.4-26.3-23.6-16c-10.2 7.9-14.3 18.6-13.7 31.1.2 3.9-.4 5.3-4.3 6.3a42.6 42.6 0 0 1-9.4 1.3 9.4 9.4 0 0 1-9-5 93.7 93.7 0 0 1-4-8.5c-4.8-11.2-14.5-15.5-26.2-11.3-4.2 1.5-18.1 11.2-18.3 11.1s-.9-2.1-1.5-5.5c-1.1-6.6-6-10.8-12.8-10.9s-11.2 3.5-19.9 1.8c-4.9-1-7.9 2.4-10 6.8-9.8 21.1-12.6 24.6-17.6 27.8-6.7 4.2-12.3.1-12.2-4.6.1-6.8 1.3-17 1.1-20a9.6 9.6 0 0 0-6.9-8.7 9.3 9.3 0 0 0-10.4 4c-2.7 4.4-6.9 29-29.4 31.5-5.2.6-8.4-2.4-7.8-7.6s3-11.1 2.6-15.8a8.9 8.9 0 0 0-9.4-8.3 8.7 8.7 0 0 0-6.6 3.5c-4 5.1-4.1 12.5-10.1 19.7s-14.4 11.6-23.4 14.5c-7.2 2.3-9.4-.1-7.9-7.6.2-1 2.5-8.3 3.3-12.4 1.8-10.3-3.2-18-13.6-20.5a55.8 55.8 0 0 0-21.9-1c-9.9 1.3-14 7.7-10.9 16.9 1 3.2.8 6.1-1.4 8.6-12.2 13.7-33.2 24.8-51.3 23.5-6-.4-9.3-4.9-8.6-10.8 1.1-10.1 9.3-19.1 17.9-24.8 2.7-1.8 4.3-1.3 6.1 1.4s5.8 5.7 10.3 5 7.5-3.7 8.9-8.1c2.3-7.2-2.5-15.6-10.4-18.2-17.2-5.8-46.2 17.3-50.6 39.8a26.2 26.2 0 0 0 20.2 30.9c25 5.7 73.2-17.5 78.5-41.8a4.2 4.2 0 0 1 4.8-3.5l.8.2c2.8.9 2.3 3.1 1.9 5.1-.7 4-1.8 7.9-2 11.9-.7 11.6 6.6 22.5 21.5 21.4 12.9-.9 24.2-6 34.5-13.4 3.5-2.5 4.5-2.6 7.5.3a21.5 21.5 0 0 0 15.8 6.1 47.5 47.5 0 0 0 28.3-9.7c3.9-2.9 4.9-3.2 7.6.7 6 8.8 11.6 13.9 20.8 11.7 14.2-3.4 18.5-10.5 32.7-32.4 2.2-3.4 3-6.1 7-6.7l2.1-.4c4.2-.8 5.1.2 4.6 4.3-1.5 11.6-1.9 14.9.3 19.5a6.9 6.9 0 0 0 9 3.5l.4-.2c9-4.3 13.8-15 30.7-21.6 3.5-1.4 5.5-.3 7.6 2.8s9.8 19.2 28 17.4a77.7 77.7 0 0 0 15.1-3c3.4-1.1 5.8-.6 8.9 1.1s7.7 3.9 11.8 4.3c26.5 2.6 60.8-14.4 57.5-36.9-.4-2.6.8-3.7 3.3-3.2a117.5 117.5 0 0 1 15.5 4c5.7 1.9 8.5 6.2 9 12.2a56.7 56.7 0 0 0 2.2 12.3c2.2 7.3 7.3 12.1 14.8 14.5 14.8 4.9 49.2-2.3 74.8-30.8 11-11.9 4.9-24.8-3.8-32.4ZM864 60.2c-4.3 6.9 4.5 14.8 12.1 11.4 9.6-4.3 21.1-15.2 34.2-42.7 9-19-2-29.3-19.1-28.9-40.2 1-122 35.7-135.3 79.5-4.2 14 1.7 26.6 17.9 28.6 20.8 2.6 63.2-8.6 90.8 1.5 4.3 1.6 4.3 7.2 1.8 11-21.3 31.7-77.2 31.7-90.1 43-6.1 5.4-1.4 19.5 9.9 14.6 24.2-10.6 88-23.1 99.5-55.6 3.1-8.6 2.6-17.3-4.4-23.2-24.7-20.7-76.3-6-104.6-8.2-3.6-.3-5-2.3-4-5.7C783.8 47.7 850 17 890 18.4c3.4.1 4.3 1.4 2.8 4.3-13.2 24.6-23.1 28.4-28.8 37.5Z" class="cls-1"/><path d="M740.5 118.4c-26.6 21-59.5 11.8-70.2 6.7-3.4-1.6-3.5-3.1-.9-5.6 11.4-10.7 25.3-22.1 25.9-45.2.4-14.7-12.5-23.1-26.3-17.5-18 7.3-39.6 36.5-26.6 61.2 1.3 2.5.1 4.1-2 5.3-15.9 9.5-32.9 15-51.8 13.6-4.9-.4-9.7-1.4-12.4-5.4s5.7-1.9 14.5-14.4c5-7.1 11.1-19.1 2-25.5-4.8-3.4-12.2-3.1-17.1-.5-12.8 6.8-17.7 15.5-18.7 28.3-.2 2.2-.4 4.5-2.7 5.4-5.5 2.3-11.1 4-17.2 2.9s-8.2-5.1-7.4-10.4c.5-3.2 3.3-10 3.9-13.9a8.6 8.6 0 0 0-14.7-7.3c-5.7 5.5-10.6 21-24.6 31.6-2 1.5-4.1 1.6-5.9-.1-4.9-4.5-5.7-7.8-6.4-17.1-.5-7.3-7.9-11.2-15.3-10.4a29 29 0 0 0-14.6 6c-4.6 3.4-4.9 3.3-6.4-2.1-2.1-7.6-7.5-11.2-15.5-10.3-15.4 1.8-44.4 28.3-56.9 35.4-3.2 1.8-5.1.4-4.6-3.3s.6-5.1 9-23.7c2.1-4.6.4-7.8-4.4-9.2-6.8-1.9-6.9-12.2-23.1-14.4-24.6-3.4-65.2 32.8-61.1 58.5 1.5 9.4 8.6 15.7 18.2 15.5 11.8-.3 13.6-1.3 39.6-16.3 4.2-2.4 4.7-2.5 7 1.8 3.4 6.3 8.7 9.5 16.1 8.7 12-1.3 23-11.1 54.5-31.9 6.4-4.2 7.1-1.5 7.1 4.5s-.6 9.1-.8 13.6 5.5 10.1 11.6 6.2 15.1-15.8 20.6-20.5c2.7-2.3 4.8-1.4 5.6 2 1.9 8.4 7.6 13.8 14.3 18.5 4.7 3.2 9.7 4.1 15.2 1.9s10.2-6 14.6-10.1 4.4-3.5 7.7.3a27.4 27.4 0 0 0 12.9 8.5c8.5 2.6 16.8 1.5 24.9-1.1a7.9 7.9 0 0 1 8.4 1.7c8.6 6.9 21.4 12.7 47.6 8 13.1-2.4 25.1-7.9 36.1-15.1a6.9 6.9 0 0 1 8.1-.3c15.8 8.8 34.4 11.6 52.2 11.4s32.3-4.9 41.9-15.8c6.4-7.2-3.1-17.1-11.9-10.1Zm-391.2-5.8c-9.4 8.1-27.4 21.8-39.8 24.3-3.5.7-5.3-.9-5.6-4.4-.7-10.5 19.2-28 28.4-33.4 23.6-13.9 22.4 8.8 17 13.5Zm310.3-3.3c-4.8 2.7-6-.3-6.6-2.5s.1-15.9 17.5-32c4.6-4.3 11.2-4.2 9.5 2.7-4.9 20.1-17 29.9-20.4 31.8Z" class="cls-1"/></svg>
                
                <div class="">
            <div>
              <b-button v-b-modal.modal-4 style="background-color: #050505;">
                  <BIconSearch variant="secondary"/>
              </b-button>
              <b-modal id="modal-4" hide-footer hide-header
              class="my-modal" body-bg-variant="dark" body-text-variant="white" size="400"
              style="">
                <div class="d-flex flex-column justify-content-center align-items-center mb-3 mt-3">
                  <div class="h5">
                    Quickly find episodes, articles, 
                  </div>
                  <div class="h5">
                    and pages across the website.
                  </div>
                  <div class="w-100 d-block position-relative">
                    <BIconSearch class="position-absolute" variant="secondary"/>
                    <input type="text" placeholder="Search"
                    class="w-100 mt-3"
                    style="padding-left: 50px; border-color: #333333 !important; border-radius: 25px !important;">
                  </div>
                  <div class="w-100 text-white p-2 mt-2 mb-2 d-flex justify-content-center"
                  style="font-size: 20px; border: 3px solid; border-color: #333333 !important; border-radius: 25px !important; background-color: #444444;">
                    Search
                  </div>
                  <div class="d-flex justify-content-between w-100 pt-4"
                  style=" border-top: 3px solid !important; border-color: #333333;">
                    <div class="d-flex flex-column text-center">
                      <div class="rounded-circle d-flex justify-content-center align-items-center" style="height: 75px; width: 75px;">
                        <b-img src="~assets/images/popular.svg" class="" ></b-img>
                      </div>
                      Popular
                    </div>
                    <div class="d-flex flex-column text-center">
                      <div class=" rounded-circle d-flex justify-content-center align-items-center" style="height: 75px; width: 75px;">
                        <b-img src="~assets/images/latestposts.svg" class=""></b-img>
                      </div>
                      Recent
                    </div>
                    <div class="d-flex flex-column text-center">
                      <div class="rounded-circle d-flex justify-content-center align-items-center" style="height: 75px; width: 75px;">
                        <b-img src="~assets/images/topicsandtags.svg" class=""></b-img>
                      </div>
                      Browse All
                    </div>
                  </div>
                </div>
              </b-modal>
            </div>
          </div>

            </div>
            <b-collapse id="collapse-1" class="mt-2">
                <div class=" text-white text-center" style="background-color: #222222;">
                    <div class="container-fluid vh-auto p-none maxWidht text-white">
                    <div class="pb-2">Podcast</div>
                    <div class="pb-2">Newsletter</div>
                    <div class="pb-2">Topics & Tags</div>
                    <div class="pb-2">About</div>
                    <div class="pb-2">Newsroom</div>
                    <div class="pb-2">Contact</div>
                    <div class="rounded-border">
                        Subscribe
                    </div>
            </div>
                </div>
            </b-collapse>
        </div>

        <Nuxt  class="mw-100 container" style="padding: 0%;" />

        <AppFooter/>
    </div>
</template>

<script>
    import AppHeader from '../components/AppHeader'
    import AppFooter from '../components/AppFooter'
    import { BIconSearch } from 'bootstrap-vue';


    export default {
        components:{
            AppHeader,
            AppFooter,
            BIconSearch
        },
        data: () =>{
            const  mobileView = false;
            showNav: false;

            return { mobileView }
        },

        mounted() {
            this.$nextTick(() => {
            window.addEventListener('resize', this.handleView);
        })
        },

        beforeDestroy() { 
            window.removeEventListener('resize', this.handleView); 
        },

        methods: {
            handleView(){
				if (process.client) {
					this.mobileView = window.innerWidth <= 992;
                    console.log(this.mobileView);
					return this.mobileView;
				}
			}
        }
    }
</script>

<style>
 .header{
    display: flex;
 }

</style>