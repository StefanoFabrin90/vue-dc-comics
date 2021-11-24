<template>
    <footer>
        <section class="container colums">
            <div class="column-right">
                <button class="btn">Singn-up Now!</button>
            </div>
            <div class="column-left">
                <span class="follow">Follow us</span>

                <ul class="socials">
                    <li v-for="(social, index) in brandSocials" :key="`social-${index}`">
                        <a href="">
                            <img :src="social.img" :alt="`social-${index}`">
                        </a>
                    </li>
                </ul>

            </div>
        </section>
    </footer>
  
</template>

<script>
export default {
    name: 'Footer2',
    data() {
        return {
            brandSocials: [
                {
                    img:require('@/assets/footer-facebook.png'),
                    text: 'facebbok',
                },
                {
                    img:require('@/assets/footer-periscope.png'),
                    text: 'periscope',
                },
                {
                    img:require('@/assets/footer-pinterest.png'),
                    text: 'pinterest',
                },
                {
                    img:require('@/assets/footer-twitter.png'),
                    text: 'twitter',
                },
                {
                    img:require('@/assets/footer-youtube.png'),
                    text: 'youtube',
                },
            ],
        }
    },
}
</script>

<style scoped lang="scss">
footer {
    background-color: #303030;
    height: 100px;
    color: white;
}

.colums {
    display: flex;
    padding: 1rem;
    & > div {
        width: 50%;
    }
    
    .btn {
        padding: 1rem;
        font-size: 18px;
        text-transform: uppercase;
        border: 3px solid dodgerblue;
        background-color: #303030;
        color: white;
        cursor: pointer;

        &:hover {
            color: black;
            background-color: dodgerblue;
        }
    }

    .column-left {
        display: flex;
        align-items: center;

        span {
            color: dodgerblue;
            text-transform: uppercase;
            font-weight: 600;
        }
        .socials {
        display: flex;
        list-style: none;
        }

        li {
            padding: 1rem;
        }
    }

    
}

</style>