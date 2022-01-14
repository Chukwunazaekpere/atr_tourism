<template>
    <section class="d-flex about-us-container">
        <div class="mt-3 ml-4 container">
            <div class="row d-flex mt-3"></div>
            <div class="row d-flex mt-3"></div>
            <div class="row d-flex mt-3"></div>
            <div class="row">
                <div class="col-md-8">
                    <h3 class="d-flex mt-3 pl-3 about-header">About ATR</h3>
                    <div class="row d-flex about-us-text-container">
                        <span class="col-md-6">
                            <b> ATR TOURISM </b> with registered office in Lagos state Nigeria is
                            an eminent provider of Tour packages, Flight and hotel booking,
                            football trail, destination weddings, schooling abroad services,
                            travel insurance. We pride ourselves in offering world class travel
                            products. Our well experienced consultants offers clients with the
                            most economical and convenient travel solution.
                        </span>
                        <span class="col-md-5">
                            <b> ATR TOURISM </b> was incorporated on the 19th day of February 2020
                            under the corporate affair commission of the federal republic of
                            Nigeria. We help you in getting your preferred University, your
                            preferred Job in your preferred country, your preferred destination
                            for vacation. We have established a reputation in the industry for
                            having Strong and long lasting relationships with both our suppliers
                            and clients
                        </span>
                    </div>
                </div>
                <div class="col-md-4">
                    <img style="border-radius: 12px;" width="100%"  src="../assets/atr-hills.jpeg" alt="">
                </div>
            </div>
            <div class="row d-flex my-3"></div>
            <div class="row d-flex my-3"></div>
            <div class="row d-flex my-3"></div>
            <div class="row d-flex my-3"></div>
        </div>
    </section>
</template>
<script>
    export default {
        'name': "AboutUs"
    }
</script>
<style scoped>
.about-us-container {
    font-family: Georgia, 'Times New Roman', Times, serif;
    background-color: #f2f2f2;
}
.about-header {
    font-size: 40px;
    font-weight: bold;
    color: #ffce3e !important;
}
.about-us-text-container {
    color: #000;
    font-weight: 500;
    text-align: left;
    justify-content: space-between;
}
</style>