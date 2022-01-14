<template>
    <section class="choose-us-container">
        <div class="row mt-3 d-flex"></div>
        <div class="row mt-3 d-flex"></div>
        <div class="row mt-3 d-flex"></div>

        <div class="container">
            <div>
                <h3 class="mt-3 choose-us-text-header">Why Choose ATR</h3>
                <div class="row d-flex justify-content-center">
                    <p class="col-md-6 choose-us-summary-text">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus nam obcaecati non, 
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus nam obcaecati non, 
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus nam obcaecati non, 
                    </p>
                </div>
                <div class="row d-flex justify-content-center mt-4">
                    <section style="flex-direction: column;" class="animate__animated animate__bounce animate__infinite col-md-2 m-2" v-for="data in reasons" :key="data.title">
                        <img style="height: 90px; width: 90px;" :src="data.image" alt="">
                        <p class="title text-light font-weight-bold">{{data.title}}</p>
                        <span class="text-light">{{data.text}}</span>
                    </section>
                </div>
            </div>

        </div>

        <div class="row d-flex my-3"></div>
        <div class="row d-flex my-3"></div>
        <div class="row d-flex my-3"></div>
        <div class="row d-flex my-3"></div>
    </section>
</template>
<script>
    import PlaneOnGlobe from "../assets/atr-airplane-tour.png"; 
    import LocationLogo from "../assets/atr-location.png"; 
    import List from "../assets/atr-travels-list.png"; 
    import Support from "../assets/atr-support.png"; 

    export default {
        'name': "WhyChooseUs",
        data() {
            return {
                    reasons: [
                    {title: 'Properly Planned Travels', image: PlaneOnGlobe, text: "ddfdfdf"},
                    {title: 'Exceptional Planned', image: List, text: "ddfdfdf"},
                    {title: 'Timely Support', image: Support, text: "ddfdfdf"},
                    {title: 'Rated Locations', image: LocationLogo, text: "ddfdfdf"}
                ]
            }
        }
    }
</script>
<style scoped>
.choose-us-container {
    background-color: black;
    font-family: Georgia, 'Times New Roman', Times, serif;
}

.choose-us-text-header {
    color: #ffce3e !important;
    font-size: 40px;
    font-weight: bold;
}

.choose-us-summary-text {
    color: gray;
    letter-spacing: 2px;
}

.title {
    font-size: 25px;
}
</style>