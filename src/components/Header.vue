<template>
    <header>
        <section class="container section-1 display-flex justify-content">
            <a href="#">
                <img src="../assets/dc-logo.png" alt="Brand">
            </a>
            <ul>
                <li v-for="(link, index) in navLink" :key="`link-${index}`">
                    <a href="#"> {{ link.text }}</a>
                </li>
            </ul>
        </section>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            navLink: [
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
                    text: 'Collectibles',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: true,
                },
                {
                    text: 'News',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: true,
                }
            ],
        };
    },
}
</script>

<style scoped lang="scss">
.section-1 {
    margin-top: 15px;
    height: 90px;
    img {
        width: 80px;
    }
    ul {
        display: flex;
        list-style: none;
        align-items: center;
        text-transform: uppercase;
        font-size: 12px;

        li {
            height: 100%;
        }

        a {
         padding: 1rem;
         text-decoration: none;
         color: black;
         cursor: pointer;
         border-bottom: 4px solid transparent;
         height: 100%;
         align-items: center;
         display: flex;
        
         &:hover {
             border-bottom: 4px solid dodgerblue;
         }
        }
    }
}
    
</style>