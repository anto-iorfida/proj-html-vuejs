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
        <div class="row container custom-container py-5">
            <div class="col-5 text-center p-5">
                <img :src="getImageUrl('new-corner.jpg')" alt="">
                <h2>Courses</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Porro, qui facere! Excepturi recusandae, et
                    veniam sed cupiditate similique voluptatibus commodi ex omnis nemo, sequi ut, a aperiam voluptas
                    aspernatur totam?</p>
                <button class="btn-small">COURSE INFORMATION</button>
            </div>
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
    <section class="grafic">
        <div class="row py-2 gap-3 container custom-container">
            <div class="col text-center p-4">
                <div>
                    <h1>95%</h1>
                </div>
                <p>PASSAT RATE</p>
            </div>
            <div class="col text-center p-4">
                <div>
                   <h1>100%</h1>
                </div>
                <p>REFERRAL RATE</p>
            </div>
            <div class="col text-center p-4">
                <div>
                    <h1>0%</h1>
                </div>
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
    
    // background-position: top;
    // background-color: blueviolet;
    .col {
        box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
        border-radius: 10px;
        border-top: 6px solid $green-primar;
        display: flex;
        flex-direction: column;
        align-items: center;

        div {
            height: 150px;
            width: 150px;
            border-radius: 50%;
            border: 6px solid $green-primar;
            h1{
                line-height: 130px;
                color: $grey-primar;
            }
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