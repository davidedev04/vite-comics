<script>

export default {
    name: "partFooter"
}

</script>

<template>
    <footer>
        <div class="contacts">
            <div class="contactsDown">
                <div class="flexRif">
                    <div>
                        <ul>
                            <li>DC COMICS</li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <ul>
                            <li>SHOP</li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectors</li>
                        </ul>
                    </div>
                    <div class="paddMid">
                        <ul>
                            <li>DC</li>
                            <li>Terms of use</li>
                            <li>Privacy policy(New)</li>
                            <li>Ad choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscription</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact us</li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
                <div class="logoBig">
                    <img src="../assets/images/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="social">
            <div class="socialDown">
                <div>
                    <div class="buttonSign">
                        <a href="#">SIGN UP NOW!</a>
                    </div>
                </div>
                <div class="socialPart">
                    <span>FOLLOW US</span>
                    <img src="../assets/images/footer-facebook.png" alt="">
                    <img src="../assets/images/footer-twitter.png" alt="">
                    <img src="../assets/images/footer-youtube.png" alt="">
                    <img src="../assets/images/footer-pinterest.png" alt="">
                    <img src="../assets/images/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;

footer {
    width: calc(100vw - 17px);



    .contacts {
        width: 100%;
        height: 400px;
        background-image: url(../assets/images/footer-bg.jpg);
        background-size: cover;
        @include displayFlex;
        justify-content: center;

        .contactsDown {
            @include widthContent;
            @include displayFlex;
            justify-content: space-between;

            li {
                font-size: 18px;
                padding: 1px 0;
                list-style-type: none;
                color: #959595;
            }

            li:first-child {
                color: #fff;
                font-size: 23px;
                padding: 15px 0;
            }

            .flexRif {
                display: flex;

                .paddMid {
                    padding: 0 50px;
                }

            }

            .logoBig {
                height: 400px;
                overflow: hidden;

                img {
                    width: 500px;
                }

            }

        }

    }

    .social {
        width: 100%;
        height: 100px;

        background-color: #303030;
        @include displayFlex;
        justify-content: center;

        .socialDown {
            @include widthContent;
            @include displayFlex;
            justify-content: space-between;

            .buttonSign {
                border: 2px solid #0282f9;
                padding: 15px;



                a {
                    text-decoration: none;
                    color: #fff;
                }

            }


            .socialPart {
                @include displayFlex;

                span {
                    font-size: 18px;
                    color: #0282f9;
                }

                img {
                    padding-left: 10px;
                }

            }
        }

    }

    .buttonSign:hover {
        background-color: #959595;
        cursor: pointer;
    }

}
</style>