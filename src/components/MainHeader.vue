<script>

export default{
    data() {
        return{
            headerLinks:[
                {
                    id: 1,
                    name: 'Characters',
                    active: false,
                },
                {
                    id: 2,
                    name: 'comics',
                    active: true,
                },
                {
                    id: 3,
                    name: 'movies',
                    active: false,
                },
                {
                    id: 4,
                    name: 'tv',
                    active: false,
                },
                {
                    id: 5,
                    name: 'games',
                    active: false,
                },
                {
                    id: 6,
                    name: 'collectibles',
                    active: false,
                },
                {
                    id: 7,
                    name: 'videos',
                    active: false,
                },
                {
                    id: 8,
                    name: 'fans',
                    active: false,
                },
                {
                    id: 9,
                    name: 'news',
                    active: false,
                },
                {
                    id: 10,
                    name: 'shop',
                    active: false,
                },
            ]
        }
    }
}

</script>

<template>
    <header>
        <section class="container-header">
            <nav>
                <img src="../assets/img/dc-logo.png" alt="logo DC">
            </nav>
            <nav>
                <ul>
                    <li v-for="links in headerLinks" :key="headerLinks.id" :class="(headerLinks) ? 'active' : ''">
                        {{ links.name }}
                    </li>
                </ul>
            </nav>
        </section>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins' as *;

header{
    @include flex-display;

    .container-header{
    display: flex;
    align-items: center;
    justify-content: space-around;
    flex-direction: row;
    width: 100%;
        nav{
            ul{
                display: flex;
                flex-direction: row;
                    li{
                        margin: 1rem;

                    };
            };
        };
    }
};


</style>
