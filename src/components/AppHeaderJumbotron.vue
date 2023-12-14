<script>
export default {
    name: 'AppHeaderJumbotron',
}
</script>

<template>
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="jumbotron image">
    </div>
</template>

<style lang="scss" scoped>
.jumbotron {
    width: 100%;
    height: 400px;

    img {
        width: 100%;
        height: 100%;
        display: block;
        object-fit: cover;
        object-position: top;
    }

}
</style>