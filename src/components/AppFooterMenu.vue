<script>

export default {
    name: 'AppFooterMenu',
    data() {
        return {
            sitemapFooter: [
                {
                    titleSection: 'DC comics',
                    pageSection: [
                        {
                            titlePage: 'Characters',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Comics',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Movies',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'TV',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Games',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Videos',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'News',
                            linkPage: '#',
                            targetPage: '_self',
                        }
                    ]
                },
                {
                    titleSection: 'Shop',
                    pageSection: [
                        {
                            titlePage: 'Shop DC',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Shop DC Collectibles',
                            linkPage: '#',
                            targetPage: '_self',
                        }
                    ]
                },
                {
                    titleSection: 'DC',
                    pageSection: [
                        {
                            titlePage: 'Terms Of Use',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Privacy policy (New)',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Ad Choices',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Advertising',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Jobs',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Subscriptions',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Talent Workshops',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'CPSC Certificates',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Ratings',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Shop Help',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'Contact Us',
                            linkPage: '#',
                            targetPage: '_self',
                        }
                    ]
                },
                {
                    titleSection: 'Sites',
                    pageSection: [
                        {
                            titlePage: 'DC',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'MAD Magazine',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'DC Kids',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'DC Universe',
                            linkPage: '#',
                            targetPage: '_self',
                        },
                        {
                            titlePage: 'DC Power Visa',
                            linkPage: '#',
                            targetPage: '_self',
                        }
                    ]
                }
            ]
        }
    },
}

</script>

<template>
    <div class="menu" v-for="menuSection in sitemapFooter">
        <!-- Menu Title -->
        <h6>{{ menuSection.titleSection }}</h6>

        <!-- Menu List -->
        <ul>
            <!-- Menu List Item -->
            <li v-for="pageItem in menuSection.pageSection">
                <a :href="pageItem.linkPage" :target="pageItem.targetPage">{{ pageItem.titlePage }}</a>
            </li>
        </ul>

    </div>
</template>
    
<style lang="scss" scoped>
.menu {

    padding-top: 40px;
    margin-right: 80px;

    h6 {
        color: #fff;
        font-size: 26px;
        text-transform: uppercase;
        margin-bottom: 20px;
    }

    li {
        a {
            color: #959595;
            text-decoration: none;
            font-size: 16px;
            line-height: 26px;
        }
    }
}
</style>