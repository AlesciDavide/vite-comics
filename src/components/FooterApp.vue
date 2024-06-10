<script>
export default{
    data() {
        return{
            FooterLinksOne:[
                {
                    id: 1,
                    name: 'Characters',
                },
                {
                    id: 2,
                    name: 'comics',
                },
                {
                    id: 3,
                    name: 'movies',
                },
                {
                    id: 4,
                    name: 'tv',
                },
                {
                    id: 5,
                    name: 'games',
                },
                {
                    id: 6,
                    name: 'collectibles',
                },
                {
                    id: 7,
                    name: 'videos',
                },
                {
                    id: 8,
                    name: 'fans',
                },
                {
                    id: 9,
                    name: 'news',
                },
                
            ],
            FooterLinksOneShop:[
                {
                    id: 1,
                    name: 'shop DC',
                },
                {
                    id: 2,
                    name: 'shop DC collectibles',
                },
            ],
            FooterLinksTwo:[
                {
                    id: 1,
                    name: 'Terms Of Use',
                },
                {
                    id: 2,
                    name: 'Privacy policy (new)',
                },
                {
                    id: 3,
                    name: 'Ad Choices',
                },
                {
                    id: 4,
                    name: 'Advertiosing',
                },
                {
                    id: 5,
                    name: 'Jobs',
                },
                {
                    id: 6,
                    name: 'Subscriptions',
                },
                {
                    id: 7,
                    name: 'Talent Workshops',
                },
                {
                    id: 8,
                    name: 'CPS Certificates',
                },
                {
                    id: 9,
                    name: 'Ratings',
                },
                {
                    id: 10,
                    name: 'Shop help',
                },
                {
                    id: 11,
                    name: 'Contact Us',
                },
            ],
            FooterLinksThree:[
                {
                    id: 1,
                    name: 'DC',
                },
                {
                    id: 2,
                    name: 'Mag Magazine',
                },
                {
                    id: 3,
                    name: 'DC Kids',
                },
                {
                    id: 4,
                    name: 'DC Universe',
                },
                {
                    id: 5,
                    name: 'DC Power Visa',
                },
            ],

        }
    }
}
</script>

<template>
    <footer>
        <div>
            <section class="container-footer-links">
                <div>
                    <ul class="footer-links-one">
                        <h2>dc comics</h2>
                        <li v-for="links in FooterLinksOne" :key="links.id">
                            <a href="">{{ links.name }}</a>
                        </li>
                    </ul>
                    <ul class="footer-links-one-shop">
                        <h2>shop</h2>
                        <li v-for="links in FooterLinksOneShop" :key="links.id">
                            <a href="">{{ links.name }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul class="footer-links-two">
                        <h2>dc</h2>
                        <li v-for="links in FooterLinksTwo" :key="links.id">
                            <a href="">{{ links.name }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul class="footer-links-three">
                        <h2>sites</h2>
                        <li v-for="links in FooterLinksThree" :key="links.id">
                            <a href="">{{ links.name }}</a>
                        </li>
                    </ul>
                </div>
            </section>
        </div>
        <div>
            <section class="container-footer-social">
                <div class="button">
                    aaaaa
                </div>
                <div class="social">
                    zzzz
                </div>
            </section>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixins' as *;
footer{
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);
        div{
            display: flex;
            justify-content: center;
            align-items: center;
            section:nth-child(1){
                div{
                    display: flex;
                    flex-direction: column;
                    justify-content: flex-start
                };
            };
            h2{
                margin-bottom: 1rem;
                text-transform: uppercase;
            };
            ul{
                padding: 1rem;
            }
            li{
                margin-bottom: .3rem;
            }
        };
}
    .container-footer-links{
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        width: 80%;
    };
    .footer-links-one,
    .footer-links-one-shop,
    .footer-links-two,
    .footer-links-three{
        li{
            a{
                color: white;
            };
        }
    };
    .container-footer-social{
        background-color: #303030;
    };
</style>