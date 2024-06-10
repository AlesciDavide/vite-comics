<script>
export default{
    data() {
        return{
            
        }
    }
}
</script>

<template>
    <section class="container-main">
        <ul>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                digital comics
            </li>
            <li>
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                dc merchandise
            </li>
            <li>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                subscription
            </li>
            <li>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                comic shop locator
            </li>
            <li>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                dc power visa
            </li>
        </ul>

    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

.container-main{
        background-color: $main-color;
        @include flex-display;
        width: 100%;
        ul{
            padding: 1rem;
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            width: 80%;
            max-width: 1160px;
            li{
                @include flex-display;
                color: white;
                font-size: .8rem;
                text-transform: uppercase;
                img{
                    margin: 0 .8rem;
                    width: 3rem;
                }
            };
        };
}
</style>