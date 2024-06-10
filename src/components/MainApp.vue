<script>
export default{
    data() {
        return{
            
        }
    }
}
</script>

<template>
    <main>
        <section class="container-main">
            <h1>
            --> Content goes here <--
            </h1>

        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;

    main{
        background-color: #1c1c1c;
        height: 10rem;
        @include flex-display;
           
    };

    .container-main{

        h1{
                color: white;
        };
    };
</style>