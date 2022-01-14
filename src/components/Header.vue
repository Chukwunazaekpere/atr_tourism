<template>
    <div class="row">
        <div class="header mt-1">
                <header :key="item.name" v-for="item in contacts">
                <span class="col-sm-10 col-xs-10">
                    {{item.name}}:
                    {{item.value}}
                    <i :class="item.icon" ></i>
                </span>
            </header>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Header",
        data() {
            return {
                contacts: [
                    {name: "Phone", icon: "fas fa-duotone fa-phone", value: "+2348122222222"},
                    {name: "Email", icon: "fas fa-envelope-open-text", value: "tantallum@gmail.com"},
                    {name: "Office address", icon: "fas fa-map-marker-alt", value: "75 office plaza Hafnium close"},
                ]
            }
        }
    };
</script>

<style>
    .header {
        display: flex;
        justify-content: space-evenly;
        width: 100%;
        color: #ffce3e;
        font-family: Georgia, 'Times New Roman', Times, serif;
        flex-direction: row;
        font-weight: bold;
        position: sticky;
    }
    i {
        font-size: 25px;
    }
</style>

