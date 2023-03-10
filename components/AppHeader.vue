<template>
    <div class="w-100">
        <b-navbar class="h1 bg-dark d-flex justify-content-between m-0 header-up">   


            <div class="rounded-border bg-color-dark-grey d-flex justify-content-center align-items-center" style="height: 50px; width: 50px;">
                <BIconSearch variant="secondary"/>
            </div>
            <b-img src="~/assets/images/image.svg" style="width: 175px; fill: white;"></b-img>

            sabscreb
        </b-navbar>

        <b-navbar style="list-style: none;padding: 0;" class="d-flex justify-content-between
          header-bot">
            <div class="container-fluid vh-auto p-none maxWidht text-white">
                <b-nav-item class="pl-4 pr-4">Podcast</b-nav-item>
                <b-nav-item class="ml-4 mr-4">Newsletter</b-nav-item>
                <b-nav-item class="ml-4 mr-4">Topics & Tags</b-nav-item>
                <b-nav-item-dropdown text="More" right>
                    <b-dropdown-item href="#">About</b-dropdown-item>
                    <b-dropdown-item href="#">Newsroom</b-dropdown-item>
                    <b-dropdown-item href="#">Contact</b-dropdown-item>
                </b-nav-item-dropdown>
            </div>
        </b-navbar>
    </div>
  </template>
  
  <script>
    import { BIconSearch } from 'bootstrap-vue';
    
    export default {
        components:{
            BIconSearch 
        }
    }
  </script>
  
<style>
 .header-up{
    background-color:  #333333	 !important;
 }

 .header-bot{
    background-color: #222222 !important;
 }

 .maxWidht{
    max-width: 1400px;
 }

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
</style>

