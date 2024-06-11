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
        height: 500px;
        background-image: url(../assets/img/jumbotron.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;

            div{
                background-color: #0282f9;
                width: 130px;
                height: 50px;
                @include flex-display;
                position: absolute;
                top: 475px;
                left: 200px;
            }
    }
</style>