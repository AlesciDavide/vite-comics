<script>
import ListProducts from './ListProducts.vue';

export default{
    data() {
        return{
            
        }
    },
    components:{
        ListProducts,
    }
}
</script>

<template>
    <main>
            <ListProducts/>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;

    main{
        background-color: #1c1c1c;
        
        @include flex-display;
    };

</style>