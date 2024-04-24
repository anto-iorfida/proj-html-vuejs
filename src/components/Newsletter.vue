<script>
export default {
    name: "Newsletter",
    data() {
        return {

        }
    }
}
</script>

<template>
        <!-- SECTION WITH POSSIBILITY OF REGISTRATION TO NEWSLETTERE -->
    <section>
    <div class="row container custom-container text-center">
        <h2>Sign up to our Newsletter</h2>
        <div class="col"></div>
        <div class="col-8 d-flex flex-column gap-4 mt-5">
            <div class="form-floating ">
                <input type="email" class="form-control" id="floatingInput" >
                <label for="floatingInput">Email address</label>
            </div>
            <button class="btn-small">SUBSCRIBE</button>
            <p>(We do not share your data with anybody, and only use it for its intended purpose)</p>
        </div>
        <div class="col"></div>
    </div>
</section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

h2{
    color: $black-primar;
}
p,label{
    color: $grey-primar;
}

section{
    padding: 50px;
    background-image: url('../assets/img/newsletter_background.jpg');
    background-size: cover;
}

</style>
