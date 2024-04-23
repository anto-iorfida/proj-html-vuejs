<script>
export default {
    name: "InfoInstructors",
    data() {
        return {

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
        <div class="row my-5 container custom-container py-3">
            <div class="col-8">
                <h2>Your Instructors</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi aliquam dolorum blanditiis quas
                    modi repellendus praesentium magnam excepturi cum voluptatibus temporibus laborum voluptate
                    aspernatur ratione nulla labore quasi, odit nesciunt.</p>
            </div>
            <div class="col-3 d-flex justify-content-center align-items-center ">
                <div class="btn-small" width="100%">MORE ABOUT US</div>
            </div>
        </div>
        <div class="row container custom-container gap-3">
            <div class="col">
                <img :src="getImageUrl('instructor-mikehart-200x127.jpg')" alt="">
                <h5>Mike Hart</h5>
                <div class="icon">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                </div>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem ratione deleniti aliquam </p>
            </div>
            <div class="col">
                <img :src="getImageUrl('instructor-johnsmith-200x127.jpg')" alt="">
                <h5>John Smith</h5>
                <div class="icon">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                </div>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem ratione deleniti aliquam at</p>
            </div>
            <div class="col">
                <img :src="getImageUrl('instructor-angelahart-200x127.jpg')" alt="">
                <h5>Angela Hart</h5>
                <div class="icon">
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                </div>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem ratione deleniti aliquam </p>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

p {
    color: $grey-primar;
}

h2,
h5 {
    color: $black-primar;
}

section {
    margin-top:80px;

    .col {
        box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
        border-radius: 10px;
        background-color: white;
        border-top: 6px solid $green-primar;
        text-align: center;
        padding: 26px;
        position: relative;
        top: 30px;

        img {
            max-width: 200px;
        }

        h5 {
            margin: 18px 0;
            font-weight: 500;
        }

        .icon {
            display: flex;
            justify-content: center;
            gap: 14px;
            margin-bottom: 10px;
            color: $grey-primar;

        }
    }
}
</style>