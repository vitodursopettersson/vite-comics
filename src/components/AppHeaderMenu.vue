<script>

export default {
    name: 'AppHeaderMenu',
    data() {
        return {
            menu: [
                {
                    title: 'characters',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'comics',
                    link: '#',
                    target: '_self',
                    active: true,
                    visible: true,
                },
                {
                    title: 'movies',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'tv',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'games',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'collectibles',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'videos',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'fans',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'news',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },
                {
                    title: 'shop',
                    link: '#',
                    target: '_self',
                    active: false,
                    visible: true,
                },

            ]
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="menuItem in menu" :class="{ active: menuItem.active }">
            <a :href="menuItem.link" :target="menuItem.target">{{ menuItem.title
            }}</a>
        </li>
    </ul>
</template>

<style lang="scss" scoped>
.active {
    border-bottom: 6px solid #0A7CEC;
}

ul {
    display: flex;
    gap: 20px;

    li {
        display: flex;
        align-items: center;
        height: 120px;
        border-bottom: 6px solid #fff;
    }

    a {
        text-decoration: none;
        color: #464646;
        text-transform: uppercase;
        font-weight: 500;
        font-size: 13px;
    }

    li:hover a {
        color: #0A7CEC;
    }

}
</style>