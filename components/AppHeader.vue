<template>
    <div>
        <b-navbar class="h1 bg-dark d-flex justify-content-between m-0">   
            <!-- jangan lupa popupsearch maxwidht 1400 -->
            <BIconSearch variant="secondary"/>
            <div class="text-danger">
                Icon
            </div>
            sabscreb
        </b-navbar>

        <b-navbar style="list-style: none;padding: 0;" class="d-flex justify-content-between
         bg-secondary">
        <div class="container-fluid bg-danger vh-auto p-none maxWidht">
            <b-nav-item class="ml-4 mr-4">Podcast</b-nav-item>
            <b-nav-item class="ml-4 mr-4">Newsletter</b-nav-item>
            <b-nav-item class="ml-4 mr-4">Topics & Tags</b-nav-item>
            <b-nav-item class="ml-4 mr-4">More</b-nav-item>
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
 .header{
    display: flex;
 }

 .maxWidht{
    max-width: 1400px;
 }
</style>

