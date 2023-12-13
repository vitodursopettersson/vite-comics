<script>

import AppFooterBannerMenu from './AppFooterBannerMenu.vue';
import AppFooterMain from './AppFooterMain.vue';
import AppFooterBottom from './AppFooterBottom.vue';

export default {
    name: 'AppFooter',
    components: {
        AppFooterBannerMenu,
        AppFooterMain,
        AppFooterBottom,
    }
}

</script>
<template>
    <footer>

        <AppFooterBannerMenu />
        <AppFooterMain />
        <AppFooterBottom />

    </footer>
</template>

<style scoped></style>