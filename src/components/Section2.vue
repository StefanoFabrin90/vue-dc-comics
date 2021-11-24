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
                    img: require('@/assets/buy-comics-digital-comics.png'),
                    text: 'Digital Comics'
                },
                {
                    img: require('@/assets/buy-comics-merchandise.png'),
                    text: 'DC Merchandise'
                },
                {
                    img: require('@/assets/buy-comics-subscriptions.png'),
                    text: 'Subscription'
                },
                {
                    img: require('@/assets/buy-comics-shop-locator.png'),
                    text: 'Comic shop locator'
                },
                {
                    img: require('@/assets/buy-dc-power-visa.svg'),
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
                padding: 20px;
                
                li {
                    display: flex;
                    img {
                    width: 70px;
                    height: 75px;
                    padding: 5px;
                    margin-left: 40px;
                    }

                    span {
                        display: flex;
                        align-items: center;
                        text-transform: uppercase;
                        font-size: 12px;
                    }
                }
                    
            }
                
        }
         
    }
    

</style>