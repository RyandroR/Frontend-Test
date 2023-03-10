<template>
    <div>
        <AppHeader v-if="!handleView()" />

        <div class="" v-if="handleView()">
        
        </div>

        <Nuxt  class="mw-100 container" style="padding: 0%;" />

        <AppFooter/>
    </div>
</template>

<script>
    import AppHeader from '../components/AppHeader'
    import AppFooter from '../components/AppFooter'

    export default {
        components:{
            AppHeader,
            AppFooter
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