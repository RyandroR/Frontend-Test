<template>
    <div>
        <AppHeader />
        <Nuxt />
    </div>
</template>

<script>
    import AppHeader from '../components/AppHeader'

    export default {
        components:{
            AppHeader
        }
    }
</script>

<style>
 .header{
    display: flex;
 }
</style>