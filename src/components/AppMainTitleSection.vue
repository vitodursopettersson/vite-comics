<script>
export default {
    name: 'AppMainTitleSection',
    props: {
        textSection: String,
    }
}
</script>

<template>
    <div class="title-container">
        <h3>{{ textSection }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.title-container {
    width: fit-content;
    background-color: #0A7CEC;
    padding: 10px 30px;

    h3 {
        color: #fff;
        font-size: 19px;
        font-weight: 700;
        text-transform: uppercase;
    }
}
</style>