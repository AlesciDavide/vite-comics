<script>
export default{
    data() {
        return{
            
        }
    }
}
</script>

<template>

    <section class="container-jumbo">
        <div><p>current series</p></div>
    </section>

</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
    section.container-jumbo{
        width: 100%;
        height: 300px;
        background-image: url(../assets/img/jumbotron.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;

            div{
                background-color: #0282f9;
                padding: 1rem;
                @include flex-display;
                position: absolute;
                top: 275px;
                left: 170px;
                p{
                    text-transform: uppercase;
                    color: white;
                    font-size: 1.5rem
                };
            }
    }
</style>