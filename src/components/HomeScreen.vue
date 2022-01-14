<template>
    <Banner />
    <AboutUs />
    <Mission />
    <WhyChooseUs />
</template>
<script>
    import Banner from "./Banner.vue";
    import AboutUs from "./AboutUs.vue";
    import WhyChooseUs from "./WhyChooseUs.vue";
    import Mission from "./Mission.vue";
    export default {
    "name": "HomeScreen",
    components: { 
        Banner, 
        AboutUs, 
        WhyChooseUs, 
        Mission
    }
}

</script>
<style>


</style>