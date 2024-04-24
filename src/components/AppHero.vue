<script>
export default {
    name: "AppHero",
    data() {
        return {

        }
    }
}
</script>

<template>
    <!-- SECTION WITH IMG AND TEXT INFO -->
    <section>
        <div class="row container custom-container ">
            <div class="col-6">
                <h1>Drive with Avada</h1>
                <h5>We offer the finest driving tuition money can buy</h5>
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-image: url('../assets/img/homepage-hero-background.jpg');
    background-size: cover;
    min-height: 500px;
    display: flex;
    color: white;
    align-items: center;
    h1{
        font-size: xxx-large;
    }

    
}
</style>