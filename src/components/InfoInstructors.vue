<script>
export default {
    name: "InfoInstructors",
    data() {
        return {

        }
    }
}
</script>

<template>
    <section>
        <div class="row container custom-container py-3">
            <div class="col-8">
                <h2>Your Instructors</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi aliquam dolorum blanditiis quas
                    modi repellendus praesentium magnam excepturi cum voluptatibus temporibus laborum voluptate
                    aspernatur ratione nulla labore quasi, odit nesciunt.</p>
            </div>
            <div class="col d-flex justify-content-center align-items-center ">
                <div class="btn-small" width="100%">MORE ABOUT US</div>
            </div>
        </div>
        <div class="row container custom-container gap-3">
            <div class="col">
                <img src="" alt="">
                <h5></h5>
                <div>

                </div>
                <p></p>
            </div>
            <div class="col">
                <img src="" alt="">
                <h5></h5>
                <div>

                </div>
                <p></p>
            </div>
            <div class="col">
                <img src="" alt="">
                <h5></h5>
                <div>

                </div>
                <p></p>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

p {
    color: $grey-primar;
}

.col {
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    border-radius: 10px;
    background-color: white;
    border-top: 6px solid $green-primar;
}
</style>