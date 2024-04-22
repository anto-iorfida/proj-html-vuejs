<script>
import infoHeader from './infoHeader.vue';


export default {
    name: "AppHeader",
    components: {
        infoHeader

    },
    data() {
        return {
            infoHeader: [
                {
                    name: 'home'
                },
                {
                    name: 'about'
                },
                {
                    name: 'prices'
                },
                {
                    name: 'courses'
                },
                {
                    name: 'location'
                },
                {
                    name: 'blog'
                }
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <header>
        <nav class="container-lg d-flex justify-content-between align-items-center p-4">

            <div class="img-header">
                <img :src="getImageUrl('avada-drivers-logo-2x-200x39.png')" alt="logo">
            </div>
            <ul class="d-flex gap-4 ">
                <infoHeader v-for="singleInfo in infoHeader" :infoHeader="singleInfo"></infoHeader>
            </ul>

            <button class="btn-small">BOOK NOW</button>

        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;
header{
    background-color: $grey-primar;
    ul li:nth-child(4)::after {
        content: "New";
        background-color: $green-primar;
        font-size: xx-small;
        margin-left: 6px;
        padding: 2px 4px;
        border-radius: 6px;
}
}
</style>