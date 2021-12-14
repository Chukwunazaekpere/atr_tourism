<template>
    <div class="banner_style" data-aos="fade" data-stellar-background-ratio="0.5">
        <BannerContent />
    </div>
</template>

<script>
    import BannerContent from "./BannerContent.vue";

    export default {
    name: "Banner",
    components: { 
        BannerContent 
    }
}
</script>

<style>
    .banner_style {
        display: flex;
        width: 100%;
        background-image: url("../assets/banner.jpeg");
        background-size: cover;
        background-position: center;
        height: 90vh;
    }
</style>