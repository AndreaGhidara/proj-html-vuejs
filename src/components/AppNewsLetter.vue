<script >


export default {
    components: {
        nome: "AppNewsLetter"
    }
}
</script>

<template>
    <div class="boxed d-flex">
        <div class="container d-flex align-items-center ">
            <h2 class="pe-5 ps-5  fs-2 text-end">
                NewsLetter to get <br>
                in touch
            </h2>

            <div class="test d-flex align-items-center ms-5 h-25 w-50">
                Your e-mail
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
$BluRoyale: #1972F5;

    .boxed{
        height: 200px;
        background-color: $BluRoyale;
        background-image: url(../assets/img/artist-shape-color-paint-bottom-right.png), url(../assets/img/artist-shape-color-paint-top-left.png);
        background-repeat: no-repeat, no-repeat;
        background-position: 100% 100%, -0% 0% ;
    }

    .test{
        margin: 0;
        padding: 0;
        border-bottom: 1px solid black;
    }
</style>
