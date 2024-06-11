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
            margin-bottom: 3rem;

            img{
                width: 100%;
                aspect-ratio: 1/1;
                margin-bottom: .7rem;
                
            };
            p{
                color: white;
            }
        }
</style>