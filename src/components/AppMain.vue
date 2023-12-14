<script>
import AppMainTitleSection from './AppMainTitleSection.vue';
import AppMainContainerSeriesCards from './AppMainContainerSeriesCards.vue';
import AppMainButton from './AppMainButton.vue';

export default {
    name: 'AppMain',
    components: {
        AppMainTitleSection,
        AppMainContainerSeriesCards,
        AppMainButton,
    },
    data() {
        return {
            text: 'Current Series'
        }
    }
}

</script>
<template>
    <main>
        <div class="title-section container">
            <AppMainTitleSection :textSection="text" />
        </div>
        <AppMainContainerSeriesCards />
        <div class="cta-section">
            <AppMainButton />
        </div>
    </main>
</template>
<style scoped>
main {
    padding-bottom: 20px;
}

.title-section {
    margin-top: -20px;
}

.cta-section {
    text-align: center;
}
</style>