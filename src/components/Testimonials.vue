<script>
export default {
    name: "Testimonials",
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
        <div class="row container custom-container text-center ">
            <h2>Testimonials</h2>
            <p>Here's what our happy drivers had to say about our services:</p>
            <div id="carouselExampleFade" class="carousel slide carousel-fade" data-bs-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img :src="getImageUrl('testimonial-grant.png')" class="d-block w-100" alt="testimonial">
                        <p>"I had a fantastic experience with Avada Driving School. Their instructors are patient,
                            thorough, and passionate about what they do. They provided me with the knowledge and skills
                            I needed to pass my driving test on the first try. I can't thank them enough!"</p>
                        <h6>Grant Smith</h6>
                    </div>
                    <div class="carousel-item">
                        <img :src="getImageUrl('testimonial-sophia.png')" class="d-block w-100" alt="testimonial">
                        <p>"Avada Driving School really helped build my confidence behind the
                            wheel and with driving in general, and they got me a first time pass!
                            Highly recommended"</p>
                        <h6>Sophia Jones</h6>
                    </div>
                    <div class="carousel-item">
                        <img :src="getImageUrl('testimonial-kelly.png')" class="d-block w-100" alt="testimonial">
                        <p>"I couldn't be happier with my experience at Avada Driving School. Their instructors are
                            patient and knowledgeable, and they helped me become a confident and safe driver. I passed
                            my test with flying colors thanks to their guidance!"</p>
                        <h6>Kelly Roger</h6>
                    </div>
                    <div class="carousel-item">
                        <img :src="getImageUrl('testimonial-kate.png')" class="d-block w-100" alt="testimonial">
                        <p>"Avada Driving School exceeded my expectations. Their instructors are professional and
                            supportive, and they provided me with the skills and confidence I needed to pass my driving
                            test. I highly recommend them to anyone looking to learn how to drive."</p>
                        <h6>Kate Morrow</h6>
                    </div>
                    <div class="carousel-item">
                        <img :src="getImageUrl('testimonial-harold.png')" class="d-block w-100" alt="testimonial">
                        <p>"Thanks to Avada Driving School, I finally feel comfortable behind the wheel. Their
                            instructors are friendly and experienced, and they helped me overcome my driving anxiety.
                            I'm grateful for their support and would recommend them to anyone."</p>
                        <h6>Harold Tonny</h6>
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleFade"
                    data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleFade"
                    data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

p {
    color: $grey-primar;
}

h6,
h2 {
    color: $black-primar;
}

section {
    background-image: url('../assets/img/testimonial-background.jpg');
    background-size: cover;
    padding: 50px;

    .carousel-item {
        padding: 0 100px;
        display: flex;
        align-items: center;
        flex-direction: column;

        img {
            max-width: 150px;
        }

        * {
            margin: 30px 0;
        }
    }
}
</style>