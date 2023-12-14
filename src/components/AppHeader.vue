<script>

import AppHeaderLogo from './AppHeaderLogo.vue';
import AppHeaderMenu from './AppHeaderMenu.vue';
import AppHeaderJumbotron from './AppHeaderJumbotron.vue';
export default {
    name: 'AppHeader',
    components: {
        AppHeaderLogo,
        AppHeaderMenu,
        AppHeaderJumbotron,
    }
}

</script>

<template>
    <header>
        <div class="container">
            <AppHeaderLogo />
            <AppHeaderMenu />
        </div>
        <AppHeaderJumbotron />
    </header>
</template>

<style lang="scss" scoped>
header {
    background-color: #fff;
}

.container {
    justify-content: space-between;
    align-items: center;
}
</style>