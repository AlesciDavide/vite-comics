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
        <div class="second-footer">
            <section class="container-footer-social">
                <div class="button">
                    <span class="button-footer">sign-up now!</span>
                </div>
                <div class="social">
                    <h3>fallow us</h3>
                    <ul>
                        <li>
                            <img src="../assets/img/footer-facebook.png" alt="Facebook">
                        </li>
                        <li>
                            <img src="../assets/img/footer-twitter.png" alt="Twitter">
                        </li>
                        <li>
                            <img src="../assets/img/footer-youtube.png" alt="youTube">
                        </li>
                        <li>
                            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                        </li>
                        <li>
                            <img src="../assets/img/footer-periscope.png" alt="Periscope">
                        </li>
                    </ul>
                </div>
            </section>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
footer{
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);

        div:nth-child(1){
            display: flex;
            justify-content: center;
           

            section:nth-child(1){
                div{
                    display: flex;
                    flex-direction: column;
                    align-items: flex-start;
                };
            };
            h2{
                margin-bottom: 1rem;
                text-transform: uppercase;
            };
            ul{
                padding: 1rem 0;
            }
            li{
                margin-bottom: .3rem;
            }
        };
};


    .container-footer-links{
        background-repeat: no-repeat;
        background-size: cover;
        display: flex;
        width: 80%;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
        background-size: contain;
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

    .second-footer{
        background-color: #303030;
        display: flex;
        align-items: center;
        justify-content: center;
        width: 100%;
        
    };

    .container-footer-social{
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        width: 80%;
        padding: 2rem 0;
            div{
                @include flex-display;
            }
    };

    .button-footer{
        padding: 1rem 1.5rem;
        border: 2px solid $main-color;
        text-transform: uppercase;
    }

    .social{
        h3{
            text-transform: uppercase;
            color: $main-color;
        };
        ul{
            display: flex;
            flex-direction: row;
            li{
                padding-left: 1rem;
            };
        };
    };
</style>