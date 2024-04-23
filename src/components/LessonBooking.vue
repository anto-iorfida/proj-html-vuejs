<script>
export default {
    name: "LessonBooking",
    data() {
        return {

        }
    }
}
</script>

<template>
    <section>
        <div class="row container custom-container">
            <div class="info-lesson col-6 py-5">
                <h2>Get Behind The Wheel</h2>
                <p class="lh-lg">Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae doloribus officia velit
                    id autem
                    veritatis nam. Maxime cupiditate cumque, delectus itaque et?</p>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae doloribus officia velit id autem
                    veritatis nam. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Aut magni dicta cupiditate,
                    exercitationem reprehenderit deserunt, accusamus aliquid eaque repellat laborum nam mollitia
                    architecto? Eos enim ad excepturi, sapiente corporis itaque!</p>
            </div>
            <div class="col-6">
                <div class="booking lh-lg text-center p-4">
                    <h3>First Lesson Free!</h3>
                    <p>When you make a block booking with us your first lesson is included free.</p>
                    <form class="row g-3 needs-validation" novalidate>
                        <div class="col-md-6">
                            <input type="text" class="form-control" id="validationCustom01" placeholder="First name"
                                required>
                        </div>
                        <div class="col-md-6">
                            <input type="text" class="form-control" id="validationCustom02" placeholder="Last name"
                                required>
                        </div>
                        <div class="col-md-4">
                            <select class="form-select" id="validationCustom04" required>
                                <option selected disabled value="">+</option>
                                <option>+39</option>
                                <option>+49</option>
                                <option>+36</option>
                                <option>+34</option>
                                <option>+19</option>
                                <option>+09</option>
                                <option>+48</option>
                            </select>
                        </div>
                        <div class="col-md-8">
                            <input type="text" class="form-control" id="validationCustom02" placeholder="Number"
                                required>
                        </div>
                        <div class="col-md-12">
                            <input type="text" class="form-control" id="validationCustom03" placeholder="Email.."
                                required>
                        </div>
                        <div class="col-md-8">
                            <input type="text" class="form-control" id="validationCustom03" placeholder="City" required>
                        </div>
                        <div class="col-md-4">
                            <select class="form-select" id="validationCustom04" required>
                                <option selected disabled value="">Region</option>
                                <option>Calabria</option>
                                <option>Sicilia</option>
                                <option>Toscana</option>
                                <option>Sardegna</option>
                                <option>Basilicata</option>
                                <option>Puglia</option>
                                <option>Lombardia</option>
                                <option>Emilia-Romagna</option>
                                <option>Lazio</option>
                                <option>Piemonte</option>
                                <option>Veneto</option>
                                <option>Campania</option>
                                <option>Marche</option>
                                <option>Umbria</option>
                                <option>Friuli-Venezia Giulia</option>
                                <option>Molise</option>
                                <option>Trentino-Alto Adige/Südtirol</option>
                                <option>Valle d'Aosta/Vallée d'Aoste</option>
                                <option>Abruzzo</option>
                                <option>Liguria</option>
                            </select>
                        </div>
                        <div class="col-12 text-start">
                            <div class="form-check">
                                <input class="form-check-input" type="checkbox" value="" id="invalidCheck" required>
                                <label class="form-check-label" for="invalidCheck">
                                    Agree to terms and conditions
                                </label>
                            </div>
                        </div>
                        <div class="col-12">
                            <button class="btn-small" type="submit">REQUEST A CALLBACK</button>
                        </div>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

h3 {
    color: $green-primar;
}

p,
label {
    color: $grey-primar;
}

h2 {
    color: $black-primar;
}

.info-lesson {
    p {
        &:first-of-type {
            margin-top: 20px;
            font-size: large;
        }
    }
}

.booking {
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
    border-radius: 10px;
    position: relative;
    bottom: 40px;
    background-color: white;

}
</style>