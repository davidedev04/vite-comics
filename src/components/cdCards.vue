<script>

export default {
    name: "cdCards",
    props: {
        sections: Object
    }
}

</script>

<template>
        <div class="comic-card">
            <div class="imgW">
                <img :src="sections.thumb" alt="">
            </div>
            <h3>{{ sections.series }}</h3>
        </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
    
    .comic-card {
    width: calc(100% / 6 - 30px);
    height: calc(100% / 3 - 30px);
    margin: 15px;

        .imgW{
            width: 100%;
            height: 100%;

            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
            }

        }

        h3{
            color: #fff;
            margin-top: 10px;
        }

}

</style>