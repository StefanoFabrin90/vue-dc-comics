<template>
    <footer>
        <section class="container colums padding">
            <div class="colum-right">
                <div class="footer-link">
                    <div>
                        <h4>Dc Comics</h4>
                        <ul>
                            <li v-for="(Comic, index) in ComicsLink" :key="`Comic-${index}`">
                                <a href=""> {{ Comic.text }} </a>
                            </li>
                        </ul>
                        <h4>Shop</h4>
                        <ul>
                            <li v-for="(Shop, index) in ShopLink" :key="`Shop-${index}`">
                                <a href=""> {{ Shop.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>Dc</h4>
                        <ul>
                            <li v-for="(About, index) in DcLink" :key="`About-${index}`">
                                <a href=""> {{ About.text }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>Sites</h4>
                        <ul>
                            <li v-for="(Site, index) in SitesLink" :key="`Site-${index}`">
                                <a href=""> {{ Site.text }} </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="colum-left">
                <!-- <img src="../assets/dc-logo-bg.png" alt="brand-logo"> -->
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'Footer1',
    data() {
        return {
            ComicsLink: [
                {
                    text: 'Characters',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Tv',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: true,
                },
                {
                    text: 'News',
                    url: '#',
                    current: true,
                },
            ],

            DcLink: [
                {
                    text: 'Team of Use',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Advertising',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Jobs',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Talent Workshops',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Ratings',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Shop Help',
                    url: '#',
                    current: true, 
                },
                {
                    text: 'Contact us',
                    url: '#',
                    current: true, 
                },
            ],

            SitesLink: [
                {
                    text: 'DC',
                    url: '#',
                    current: true,
                },
                {
                    text: 'MAD Magazine',
                    url: '#',
                    current: true,
                },
                {
                    text: 'DC Kids',
                    url: '#',
                    current: true,
                },
                {
                    text: 'DC Universe',
                    url: '#',
                    current: true,
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                    current: true,
                },
            ],

            ShopLink: [
                {
                    text: 'Shop DC',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                    current: true,
                },
            ],
        };
    },
}
</script>

<style scoped lang="scss">
footer {
    background-image: url('../assets/footer-bg.jpg');
    width: 100%;
    height: 100%;
    object-fit: cover;
    background-size: 100%;
    background-position: center center;
}
.colums {
    
    display: flex;
    & > div {
        width: calc(100% / 2);
    };

    .footer-link {
        display: flex;
        & > div {
            width: calc(100% / 3);
        };

        h4 {
            font-size: 1.7rem;
            font-weight: 600;
            margin: 30px 0;
            text-transform: uppercase;
            color: white
        };

        ul {
            display: inline-block;
            list-style: none;

            li {
                padding: 5px 0;
            }
            a {
                text-decoration: none;
                color: lightgrey;
                font-size: 0.9rem;

                &:hover {
                    text-decoration: underline;
                }
            }
        }
    }

    .colum-left {
        background-image: url('../assets/dc-logo-bg.png');
        overflow: hidden;
        // background-repeat: no-repeat;
        background-position: center;
    }
}


</style>