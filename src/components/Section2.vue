<template>
    <section class="main-second">
        <div class="section2 container padding">
            <ul>
                <li v-for="(image, index) in brandImg" :key="`image-${index}`">
                    <img :src="image.img" :alt="`image-${index}`">
                    <span> {{image.text}} </span>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Section2',
    data() {
        return {
            brandImg: [
                {
                    img: '@/assets/buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    img: '@/assets/buy-comics-digital-comics.png',
                    text: 'DC Merchandise'
                },
                {
                    img: '@/assets/buy-comics-digital-comics.png',
                    text: 'Subscription'
                },
                {
                    img: '@/assets/buy-comics-digital-comics.png',
                    text: 'Comic shop locator'
                },
                {
                    img: '@/assets/buy-comics-digital-comics.png',
                    text: 'dc power visa'
                },
            ],
        }
    },
}
</script>

<style scoped lang="scss">
    .main-second {
        background-color: dodgerblue;
        color: white;
        
        .section2 {
            ul {
                list-style: none;
                display: flex;
                justify-content: center;
                
                li {
                    display: flex;
                    img {
                    width: 60px;
                    }

                    span {
                        display: flex;
                        align-items: center;
                        padding: 1rem;
                        text-transform: uppercase;
                        font-size: 12px;
                    }
                }
                    
            }
                
        }
         
    }
    

</style>