<script>
import AppFooterMenu from './AppFooterMenu.vue';
export default {
    name: 'AppFooterMain',
    components: {
        AppFooterMenu,
    }
}

</script>

<template>
    <!-- Main Footer -->
    <main>
        <div class="container">
            <div class="menu-container">
                <AppFooterMenu />
            </div>
            <div class="logofooter-container">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>


    </main>
</template>

<style lang="scss" scoped>
main {
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 500px;
    overflow: hidden;
}

.container {
    height: 100%;
    justify-content: space-between;
}

.menu-container {
    height: 100%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
}

.logofooter-container {

    img {
        height: 140%;
        margin-top: -10%;
    }
}
</style>