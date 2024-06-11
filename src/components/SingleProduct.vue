<script>
export default{
    data() {
        return{
            
        }
    },
    props: {
        singleProduct:{
            type: Object,
            required: true,
        }
    },
}
</script>

<template>
    <article>
        <img :src="singleProduct.thumb" :alt="singleProduct.series">
        <p>{{ singleProduct.series }}</p>
    </article>

</template>

<style scoped>
    article{
            width: calc((100% / 6) - .8rem);
            margin-right: .8rem;

            img{
                width: 100%;
                height: 60%;
                margin-bottom: .5rem;
                
            };
            p{
                color: white;
            }
        }
</style>