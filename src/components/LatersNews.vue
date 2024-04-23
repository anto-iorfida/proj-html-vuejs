<script>
export default {
    name: "LatersNews",
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
        <div class="row container custom-container text-center bg-transparent">
            <div class="row ciao">
                <h2>Latest News</h2>
                <div class="col">
                    <img :src="getImageUrl('blog-choosecar-320x202.jpg')" alt="">
                    <h5>What Car to Start With?</h5>
                    <div class="laters-period">
                        <p>February 7th, 2019 | <span>0 Comment</span></p>
                    </div>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem ratione deleniti aliquam
                    </p>
                </div>
                <div class="col">
                    <img :src="getImageUrl('blogpost-10and2-320x202.jpg')" alt="">
                    <h5>Avada Driving School Expanding</h5>
                    <div class="laters-period">
                        <p>February 7th, 2019 | <span>0 Comment</span></p>
                    </div>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem ratione deleniti aliquam
                    </p>
                </div>
                <div class="row mt-5">
                    <div class="col">
                        <button class="btn-small">MORE FROM THE BLOG</button>
                    </div>
                </div>
            </div>
            <div class="row latestnews   p-0">
                <img :src="getImageUrl('latestnews-bottom-600x52.png')" alt="">
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../style/variables' as*;

p {
    color: $grey-primar;
}

h5,
span {
    color: $green-primar;
}

section {
    background-image: url('../assets/img/latestnews-background.jpg');
    background-size: cover;

    .row {
        position: relative;
        bottom: 20px;
    }

    .row.ciao {
        background-color: white;
        border-radius: 10px 10px 0 0;
        box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
        border-top: 4px solid #7799ad;

        h2 {
            margin: 40px;
        }

        .col {


            img {
                max-width: 500px;
            }

            .laters-period {
                p {
                    font-size: x-small;

                }
            }

            * {
                margin: 10px 0;
            }
        }
    }

    .row.latestnews {
        img {
            padding: 0;
        }
    }



}
</style>