<script>
export default {
    name: 'AppFooterBottomSocial',
    data() {
        return {
            socials: [
                {
                    title: 'facebook',
                    icon: '../assets/img/footer-facebook.png',
                    link: '#',
                    target: '_self',
                },
                {
                    title: 'twitter',
                    icon: '../assets/img/footer-twitter.png',
                    link: '#',
                    target: '_self',
                },
                {
                    title: 'youtube',
                    icon: '../assets/img/footer-youtube.png',
                    link: '#',
                    target: '_self',
                },
                {
                    title: 'pinterest',
                    icon: '../assets/img/footer-pinterest.png',
                    link: '#',
                    target: '_self',
                },
                {
                    title: 'periscope',
                    icon: '../assets/img/footer-periscope.png',
                    link: '#',
                    target: '_self',
                }
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
    <div class="social-icon">
        <h6>Follow US</h6>
        <a v-for="social in socials" :href="social.link">
            <img :src="getImagePath(social.icon)" :alt="social.title" :href="social.link">
        </a>
    </div>
</template>


<style lang="scss" scoped>
.social-icon {
    display: flex;
    align-items: center;
    gap: 15px;

    h6 {
        color: #0A7CEC;
        font-size: 16px;
        text-transform: uppercase;
        margin-right: 15px;
    }
}
</style>