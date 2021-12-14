<template>
    <div class="header mt-2">
        <header :key="item.name" v-for="item in contacts">
            <span>
                {{item.name}}: 
                <i :class="item.icon" ></i>
            </span>
        </header>
    </div>
</template>

<script>
    export default {
        name: "Header",
        data() {
            return {
                contacts: [
                    {name: "Phone", icon: "fa-duotone fa-phone"},
                    {name: "Email", icon: ""},
                    {name: "Office address", icon: ""},
                ]
            }
        }
    }
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
    }
</style>

