<template>
    <div class="container" data-aos="fade-up" data-aos-delay="400">
        <Header />
        <div class="row mt-5"></div>
        <div class="row mt-md-5 mt-sm-3"></div>
        <div class="row mt-md-5 mt-sm-3"></div>
        <div class="row mt-4"></div>

        <div class="animate__animated animate__flash row mt-5 content">
            <div class="col-md-4 col-sm-12 col-xs-12 text_container">
                <span class="text-center banner_text1">ATR</span> <br />
                <span class="text-center banner_text2">Tourism</span>
                <span class="text-center banner_text3"> <br />
                    We've always delivered the best of its kind, ranging from comfort and
                    satisfaction. ATR ensures that you get more than you've given. 
                </span>
                <span class="col-6 lower_bar"></span>
            </div>
            <div class="col-md-5 col-xs-12 col-sm-12">
                <p class="form_text py-2 col-12">Talk to us...</p>
                <div class="form-group" v-for="props in fieldProps" :key="props.name" >
                    <span style="flex-direction: row;" v-if="props.type !== 'textarea'">
                        <input 
                            :placeholder="props.name" 
                            :type="props.type" 
                            class="form-control my-2"
                            required="true"
                        />
                    </span>
                    <span v-else>
                        <textarea 
                            class="form-control" 
                            :key="props.name" 
                            cols="50" rows="3" 
                            :placeholder="props.name"
                        />
                    </span>
                </div>
                <button class=" mt-2 col-3 btn btn- px-4 send_button">
                    Send
                </button>
            </div>
        </div>
    </div>
</template>

<script>
    import Header from "@/components/Header.vue";

    export default {
        name: "BannerContent",
        components: {
            Header
        },
        data() {
            return {
                fieldProps: [
                    {name: "Fullname", type: "text"}, 
                    {name:  "Email", type: "email"},
                    {name:  "Message", type: "textarea"}
                ]
            }
        }
    }
</script>

<style scoped>
    .content {
        justify-content: space-between;
    }
    .fields_container {
        /* display: flex; */
        /* width: 100%; */
        align-items: flex-end;
    }
    .form-group textarea,
    .form-group input {
        display: flex;
        justify-content: flex-end;
        border: 2px solid #fff;
        background-color: transparent;
        color: ghostwhite;
        font-size: 20px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: bold;
        /* float: right; */
    }
    .text_container {
        text-align: left;
    }
    .banner_text1 {
        font-family: Georgia;
        font-weight: bold;
        font-size: 3rem;
        letter-spacing: 7px;
        color: #ffce3e !important;
    }
    .banner_text2 {
        font-family: Georgia;
        font-weight: bold;
        font-size: 2rem;
        color: #ffce3e !important;
    }
    .banner_text3 {
        font-family: Georgia;
        font-weight: bold;
        font-size: .9rem;
        color: #f4f4f4 !important;
        text-align: left;
        font-style: italic;
    }
    button {
        background-color: #ffce3e !important;
        color: #000 !important;
        font-family: Georgia, 'Times New Roman', Times, serif;
    }
    button:hover {
        background-color: #ffce3e!important;
        border: 2px solid #fff;
    }
    .form_text {
        font-family: Georgia;
        font-weight: bold;
        font-size: 1.3rem;
        color: #ffce3e !important;
        font-style: italic;
        background-color: rgb(27, 26, 26);
        float: left;

    }
    .send_button {
        float: left;
    }
    .lower_bar {
        display: flex;
        border-bottom: 13px solid #ffce3e;
        border-radius: 10px;
    }
</style>