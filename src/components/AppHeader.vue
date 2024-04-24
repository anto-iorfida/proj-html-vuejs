<script>
import infoHeader from './infoHeader.vue';


export default {
    name: "AppHeader",
    components: {
        infoHeader

    },
    data() {
        return {
            // array object with data header
            infoHeader: [
                {
                    name: 'home',
                    id: '1'
                },
                {
                    name: 'about',
                    id: '2'
                },
                {
                    name: 'prices',
                    id: '3'
                },
                {
                    name: 'courses',
                    id: '4'
                },
                {
                    name: 'location',
                    id: '5'
                },
                {
                    name: 'blog',
                    id: '6'
                }
            ]

        }
    },
    methods: {
        // funtion to insert image
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <header>
        <!-- section ads -->
        <div class="row  ads">
            <div class="row container custom-container ">
                <div class="col">
                    <p>We have a 95% Successful Pass Rate!</p>
                </div>
                <div class="col text-end">
                    <p><i class="fa-solid fa-phone-flip"></i> Give us a call to book your tuition! 1-800-555-555 </p>
                </div>
            </div>
        </div>
        <!-- navigation bar -->
        <nav class="container custom-container d-flex justify-content-between align-items-center p-4">

            <div class="img-header">
                <img :src="getImageUrl('avada-drivers-logo-2x-200x39.png')" alt="logo">
            </div>
            <ul class="d-flex gap-4 ">
                <infoHeader v-for="(singleInfo, index) in infoHeader" :infoHeader="singleInfo" :key="singleInfo.id"
                    :currentIndex="index">
                </infoHeader>
            </ul>

            <button class="btn-small">BOOK NOW</button>

        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

p {
    color: $grey-primar;
}

header {
    background-color: rgba(73, 76, 78, 0.5);
    width: 100%;
    position: fixed;
    z-index: 20;

    // component 'New' inser word COURSES
    ul li:nth-child(4)::after {
        content: "New";
        background-color: $green-primar;
        font-size: xx-small;
        margin-left: 6px;
        padding: 2px 4px;
        border-radius: 6px;
    }

    .ads {
        background-color: #1c1d1e;

    }
}
</style>