<script>

export default {
    name: "partMiddle",

    data() {
        return {
            infos: [
                {
                    image: "../src/assets/images/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS"
                },
                {
                    image: "../src/assets/images/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {
                    image: "../src/assets/images/buy-comics-subscriptions.png",
                    text: "COMIC SHOP"
                },
                {
                    image: "../src/assets/images/buy-comics-shop-locator.png",
                    text: "SUBSCRIPTION"
                },
                {
                    image: "../src/assets/images/buy-dc-power-visa.svg",
                    text: "DC POWER VISA"
                },
            ]
        }
    }
}

</script>

<template>
    <main>
        <div class="contentMiddle">
            <div class="divJumbo">
                
            </div>
        </div>
        <div class="stats">
            <div class="descrizione">
                <div v-for="info in infos" class="image_info">
                    <img :src="info.image" alt="">
                    <span>{{ info.text }}</span>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;

main {
    width: 100vw;


    .contentMiddle {
        width: 100%;
        height: 500px;
        background-image: url(../assets/images/jumbotron.jpg);
    }

    .stats {
        width: 100%;
        height: 150px;
        background-color: #0282f9;
        @include displayFlex;
        justify-content: center;

        .descrizione {
            width: 80%;
            @include displayFlex;
            justify-content: space-between;

            .image_info {
                @include displayFlex;

                img {
                    width: 40px;
                    height: 40px;
                    margin-right: 8px;
                    object-fit: contain;
                }

                span {
                    color: #fff;
                }

            }

        }

    }
}
</style>