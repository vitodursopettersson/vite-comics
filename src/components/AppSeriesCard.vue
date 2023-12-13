<script>
export default {
    name: 'AppSeriesCard',
    props: {
        img: String,
        title: String,
    }
}

</script>

<template>
    <div class="card">
        <a href="#">
            <div class="img-container">
                <img :src="img" :alt="title">
            </div>
            <h5>{{ title }}</h5>
        </a>

    </div>
</template>

<style lang="scss" scoped>
.card {
    width: 200px;

    a {
        text-decoration: none;
    }

    &:hover h5 {
        text-decoration: underline;
    }

    .img-container {

        width: 200px;
        height: 200px;
        position: relative;
        margin-bottom: 14px;

        img {
            width: 100%;
            height: 100%;
            display: block;
            object-fit: cover;
            object-position: top;
        }
    }

}

h5 {
    color: #fff;
    text-transform: uppercase;
    font-weight: 400;
}
</style>