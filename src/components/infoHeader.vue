<script>
export default {
    name: "infoHeader",
    props: {
        infoHeader: Object
    },
}
</script>

<!-- single info in header (AppHeader) -->
<template>
    <li><a href="">{{infoHeader.name}}</a></li>
</template>

<style lang="scss" scoped>
li{
    color: white;
    text-transform: uppercase;
    font-size: small;
    font-weight: 500;
    padding: 6px;
}
</style>