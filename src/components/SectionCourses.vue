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
        <div class="row container custom-container">
            <div class="col-5 text-center p-5">
                <h2>Courses</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Porro, qui facere! Excepturi recusandae, et
                    veniam sed cupiditate similique voluptatibus commodi ex omnis nemo, sequi ut, a aperiam voluptas
                    aspernatur totam?</p>
                <button class="btn-small">COURSE INFORMATION</button>
            </div>
            <div class="col">
                <img src="" alt="">
                <h5></h5>
                <button class="btn-info"></button>
            </div>
            <div class="col">
                <img src="" alt="">
                <h5></h5>
                <button class="btn-info"></button>
            </div>
            <div class="col">
                <img src="" alt="">
                <h5></h5>
                <button class="btn-info"></button>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped></style>