<script>
    export default {
        name: "InfoNumber",
        data(){
                return{

                }
            } 
        }
</script>

<template>
<section>
    <!-- SECTION WITH INFO NUMBERS FOR BOOKING LESSON -->
    <div class="row container custom-container py-5">
        <div class="col-6">
            <h2>Start Learning to Drive Today</h2>
            <p>Give us a call to schedule your first driving lesson</p>
        </div>    
        <div class="col-6 align-items-center d-flex justify-content-center gap-3">
            <h2>
                <i class="fa-solid fa-phone-flip"></i>
                <a href="">1-800-555-555</a>
            </h2>
        </div>
    </div>
</section>
</template>

<style lang="scss" scoped>
section{
    background-image: url('../assets/img/horizontal-cta-background.jpg');
    background-size: cover;
    color: white;
    .fa-phone-flip{
        margin: 20px;
    }

}
</style>