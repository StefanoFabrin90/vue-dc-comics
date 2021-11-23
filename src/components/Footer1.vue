<template>
    <footer>
        <section class="container colums padding">
            <div class="colum-right">
                <div class="footer-link">
                    <div>
                        <h4>Dc Comics</h4>
                        <ul>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                        </ul>
                        <h4>Shop</h4>
                        <ul>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h4>Dc</h4>
                        <ul>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                        </ul></div>
                    <div>
                        <h4>Sites</h4>
                        <ul>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                            <li>
                                <a href="">test</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="colum-left">
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </section>
    </footer>
</template>

<script>
export default {
    name: 'Footer1'
}
</script>

<style scoped lang="scss">
footer {
    background-image: url('../assets/footer-bg.jpg');
    background-repeat: no-repeat;
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
            font-size: 1.5rem;
            margin: 30px 0;
            text-transform: uppercase;
            color: white
        };

        ul {
            display: inline-block;
            list-style: none;
            a {
                text-decoration: none;
                color: lightgrey
            }
        }
    }
}


</style>