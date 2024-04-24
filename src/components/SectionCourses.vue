<script>
export default {
    name: "SectionCourses",
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
        <!-- SECTION WITH INFO COURSES -->
        <div class="row container custom-container py-5">
            <div class="col-5 text-center p-5">
                <img :src="getImageUrl('new-corner.jpg')" alt="">
                <h2>Courses</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Porro, qui facere! Excepturi recusandae, et
                    veniam sed cupiditate similique voluptatibus commodi ex omnis nemo, sequi ut, a aperiam voluptas
                    aspernatur totam?</p>
                <button class="btn-small">COURSE INFORMATION</button>
            </div>
            <!-- SELECT COURSES ,3 TYPES OF COURSE-->
            <div class="col text-center">
                <img :src="getImageUrl('courses-passplus-200x200.jpg')" alt="auto">
                <h5>Pass Plus</h5>
                <button class="btn-info">LEARN MORE</button>
            </div>
            <div class="col text-center">
                <img :src="getImageUrl('course-intensive-200x200.jpg')" alt="auto">
                <h5>Intensive course</h5>
                <button class="btn-info">LEARN MORE</button>
            </div>
            <div class="col text-center">
                <img :src="getImageUrl('courses-instructor-200x200.jpg')" alt="auto">
                <h5>Instructors</h5>
                <button class="btn-info">LEARN MORE</button>
            </div>
        </div>
    </section>
    <!--  3 GRAFIC -->
    <section class="grafic">
        <div class="row py-2 gap-3 container custom-container">
            <div class="col text-center p-4">
                <svg class="cerchio" viewBox="0 0 100 100">
                    <circle class="bordo bordo-grigio" cx="50" cy="50" r="40"></circle>
                    <circle cx="50" cy="50" r="40" stroke-dasharray="277" stroke-dashoffset="50"></circle>
                    <text x="50%" y="50%" text-anchor="middle" dominant-baseline="middle" fill="grey">95%</text>
                </svg>

                <p>PASSAT RATE</p>
            </div>
            <div class="col text-center p-4">
                <svg class="cerchio" viewBox="0 0 100 100">
                    <circle cx="50" cy="50" r="40" stroke-dasharray="301" stroke-dashoffset="50"></circle>
                    <text x="50%" y="50%" text-anchor="middle" dominant-baseline="middle" fill="grey">100%</text>
                </svg>
                <p>REFERRAL RATE</p>
            </div>
            <div class="col text-center p-4">
                <svg class="cerchio" viewBox="0 0 100 100">
                    <circle class="bordo bordo-grigio" cx="50" cy="50" r="40"></circle>
                    <circle cx="50" cy="50" r="40" stroke-dasharray="246" stroke-dashoffset="243"></circle>
                    <text x="50%" y="50%" text-anchor="middle" dominant-baseline="middle" fill="grey">1%</text>
                </svg>
                <p>ACCIDENT RATE</p>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

section {
    background-image: url('../assets/img/promise-background.jpg');
    background-size: cover;
    background-position: center;

    .row {
        .col-5 {
            box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
            position: relative;
            bottom: 80px;
            border-radius: 10px;
            background-color: white;
            overflow: hidden;

            img {
                position: absolute;
                top: 0;
                left: 0;
                max-width: 80px;
            }

            h2 {
                color: $black-primar;
            }

            p {
                color: $grey-primar;
            }
        }

        .col {
            h5 {
                color: #7799ad;
                margin: 18px 0;
                font-size: medium;
                font-weight: 500;

            }

            img {
                max-width: 130px;
            }
        }
    }
}

.grafic {
    background-image: url('../assets/img/driving-triangle.svg');
    background-size: cover;
    background-repeat: no-repeat;

    .col {
        box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
        border-radius: 10px;
        background-color: white;
        border-top: 6px solid $green-primar;
        display: flex;
        flex-direction: column;
        align-items: center;

        .cerchio {
            width: 150px;
            height: 150px;

        }

        .cerchio circle {
            fill: none;
            stroke: $green-primar;
            stroke-width: 4;
            // stroke-dasharray: 277;
            // stroke-dashoffset: 50;
            transform: rotate(270deg);
            transform-origin: center;

        }

        .cerchio .bordo-grigio {
            fill: none;
            stroke: lightgray;
            stroke-width: 4;
        }

        .cerchio text {
            color: gray;
            font-size: 20px;
            font-weight: 500;
        }

        p {
            color: $grey-primar;
            font-weight: 500;
            font-size: small;
            margin: 30px 0;
        }
    }
}
</style>