<script>
export default {
    name: "DataFooter",
    props: {
        dataFooter: Object
    },
    data() {
        return {

        }
    }
}
</script>

<!-- INFO INSERTED DYNAMICLY -->
<template>
<li  class="d-flex gap-3"><span v-html="dataFooter.icon"></span>{{ dataFooter.name }}</li>
</template>

<style lang="scss" scoped></style>