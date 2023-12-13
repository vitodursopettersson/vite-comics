<script>

export default {
    name: 'AppFooterBannerMenu',
    data() {
        return {
            menuBannerFooter: [
                {
                    title: 'digital comics',
                    link: '#',
                    target: '_self',
                    icon: '../assets/img/buy-comics-digital-comics.png',
                    visible: true,
                },
                {
                    title: 'dc merchandise',
                    link: '#',
                    target: '_self',
                    icon: '../assets/img/buy-comics-merchandise.png',
                    visible: true,
                },
                {
                    title: 'subscription',
                    link: '#',
                    target: '_self',
                    icon: '../assets/img/buy-comics-subscriptions.png',
                    visible: true,
                },
                {
                    title: 'comic shop locator',
                    link: '#',
                    target: '_self',
                    icon: '../assets/img/buy-comics-shop-locator.png',
                    visible: true,
                },
                {
                    title: 'dc power visa',
                    link: '#',
                    target: '_self',
                    icon: '../assets/img/buy-dc-power-visa.svg',
                    visible: true,
                },
            ]
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        },
    }
}

</script>

<template>
    <!-- Section Menu Banner -->
    <div class="banner">

        <!-- Menu Item -->
        <div v-for="itemMenu in menuBannerFooter" class="banner-menu-item">

            <img :src="getImagePath(itemMenu.icon)" :alt="itemMenu.tit">
            <h6>{{ itemMenu.title }}</h6>

        </div>

    </div>
</template>

<style lang="scss" scoped>
.banner {
    background-color: #0A7CEC;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 70px;
    height: 140px;
}

.banner-menu-item {
    display: flex;
    align-items: center;
    gap: 15px;

    img {
        width: 60px;
        height: 60px;
        object-fit: contain;
    }

    h6 {
        color: #fff;
        font-size: 13px;
        font-weight: 400;
        text-transform: uppercase;
    }

}
</style>