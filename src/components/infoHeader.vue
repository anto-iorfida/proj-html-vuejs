<script>
export default {
    name: "infoHeader",
    props: {
        infoHeader: Object,
        currentIndex: Number
    },
    data() {
        return {
            // VARIABLE 0 
            activeLink: 0
        };
    },
    methods: {
        // FUNCTION  WHICH INITIALIZES VARIABLE AT ELEMENT INDEX
        getActive(index) {
            this.activeLink = index;
            console.log(index);
        }
    }
}
</script>

<!-- SINGLE INFO IN HEADER (AppHeader) -->
<template>
    <!-- UPON THE CLICK THE VARIABLE BECOMES THE INDEX OF THE ELEMENT AND THE CLASS IS ADDED -->
    <li :class="{ 'actives': currentIndex === activeLink }" @click="getActive(currentIndex)"><a href="">{{
        infoHeader.name }}</a></li>
</template>

<style lang="scss" scoped>
li {
    color: white;
    text-transform: uppercase;
    font-size: small;
    font-weight: 500;
    padding: 6px;

    
    a:hover {
        color: #7abc64;
    }
}

.actives {
    color: #7abc64;
    border-bottom: 3px solid #7abc64;
}
</style>