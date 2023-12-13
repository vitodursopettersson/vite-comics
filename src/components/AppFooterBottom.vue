<script>

import AppFooterBottomSocial from './AppFooterBottomSocial.vue';
import AppFooterBottomButton from './AppFooterBottomButton.vue';

export default {
    name: 'AppFooterBottom',
    components: {
        AppFooterBottomSocial,
        AppFooterBottomButton,
    }
}

</script>

<template>
    <section class="footer-bottom">
        <div class="container">

            <AppFooterBottomButton />
            <AppFooterBottomSocial />

        </div>
    </section>
</template>


<style lang="scss" scoped>
.footer-bottom {
    background-color: #303030;
}

.container {
    padding: 40px 0;
    justify-content: space-between;
}
</style>