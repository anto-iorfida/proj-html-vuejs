<script>
import DataFooter from './DataFooter.vue';

export default {
    name: "AppInfoFooter",
    components: {
        DataFooter
    },
    data() {
        return {
            contactFotter: [
                {
                    name: '12345 North Main Street,New York,NY 55555',
                    icon: '<i class="fa-solid fa-house-chimney"></i>'
                },
                {
                    name: '1.800.555.67.89',
                    icon: '<i class="fa-solid fa-phone-flip"></i>'
                },
                {
                    name: 'info@your-domain.com',
                    icon: '<i class="fa-solid fa-envelope"></i>'
                },
                {
                    name: 'theme-fudion.com',
                    icon: '<i class="fa-solid fa-share-nodes"></i>'
                }
            ],
            courses: [
                {
                    name: 'Pass plus',
                    icon: '<i class="fa-solid fa-circle-arrow-right"></i>'
                },
                {
                    name: 'Intensive Course',
                    icon: '<i class="fa-solid fa-circle-arrow-right"></i>'
                },
                {
                    name: 'Automatic',
                    icon: '<i class="fa-solid fa-circle-arrow-right"></i>'
                },
                {
                    name: 'Instructor Training',
                    icon: '<i class="fa-solid fa-circle-arrow-right"></i>'
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
    <section>
        <div class="row container custom-container">
            <div class="col-3">
                <img :src="getImageUrl('avada-drivers-logo-2x-200x39.png')" alt="">
                <p class="lh-lg">
                    Avada Driving School is the right choice for
                    experienced drivers looking for a refresher
                    course, or the brand new driver wanting to
                    pass first time.
                </p>
            </div>
            <div class="col-3">
                <h5>CONTACT DETAILS</h5>
                <ul class="d-flex flex-column gap-3 ">
                    <DataFooter v-for="info in contactFotter" :dataFooter="info"></DataFooter>
                </ul>
            </div>
            <div class="col-3">
                <h5>COURSES</h5>
                <ul class="d-flex flex-column gap-3">
                    <li v-for="cors in courses" class="d-flex gap-3 courses"><span v-html="cors.icon"></span>{{
                        cors.name }}
                    </li>
                </ul>
            </div>
            <div class="col-3 text-center">
                <img :src="getImageUrl('footer-ad-grid-400x357.png')" alt="">
                <button class="btn-small">BOOK NOW</button>
            </div>
        </div>
    </section>
    <section>
        <div class="row container custom-container">
            <div class="col-8 ">
            <p>© Copyright 2012 - 2020 | Avada Theme by <span>ThemeFusion</span> | All Rights Reserved | Powered by <span> WordPress</span></p>
            </div>
            <div class="col ">
                <div class="icon d-flex gap-3 text-white justify-content-end ">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-instagram"></i>
                </div>
            </div>
        </div>
    </section>
    
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

p,
li {
    color: $grey-primar;
}

li.courses,span {
    color: $green-primar;
}

h5 {
    color: white;
}

img,
h5 {
    margin-bottom: 24px
}

section:first-of-type {
    background-image: url('../assets/img/footer-background-color.jpg');
    background-size: cover;
}
.row {
    padding: 50px 0;

    img {
        max-width: 100%;
    }

}

section{
    background-color: #1c1d1e;
    p{
        font-size: small;
    }
}
</style>