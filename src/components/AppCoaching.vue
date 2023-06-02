<script >

export default {
    components: {
        nome: "AppCoaching"
    }
}
</script>

<template>
    <div class="container-fluid text-center py-5 box">
        <!-- <img class="artist-shape-1" src="../assets/img/artist-shape-01.png" alt="">
            <img class="maxcoach-shape-13" src="../assets/img/maxcoach-shape-13.png" alt="">
            <img class="maxcoach-shape-14" src="../assets/img/maxcoach-shape-14.png" alt=""> -->
        <h2 class="artist">Artist Coaching</h2>
        <h1>
            I understand what it takes to create. <br>
            I can help you with
        </h1>
        <div class="container py-5">
            <div class="row row-col-4">
                <div class="col">
                    <img src="../assets/img/artist-box-image-01.png" alt="">
                    <p>
                        <strong>
                            Online Coues
                        </strong>
                    </p>
                    <p>Online art coaching now offers you a very powerful way to redesign your artist mind.</p>
                </div>
                <div class="col">
                    <img src="../assets/img/artist-box-image-02.png" alt="">
                    <p>
                        <strong>
                            One to One
                        </strong>
                    </p>
                    <p>Getting the necessary clarity about the current state to help you improve your ability.</p>
                </div>
                <div class="col">
                    <img src="../assets/img/artist-box-image-03.png" alt="">
                    <p>
                        <strong>
                            Anywhere
                        </strong>
                    </p>
                    <p>Access to valuable and portable program which allow you to setup and live anywhere you want.</p>
                </div>
                <div class="col">
                    <img src="../assets/img/artist-box-image-04.png" alt="">
                    <p>
                        <strong>
                            One to One
                        </strong>
                    </p>
                    <p>Punctuality is our top priority because it's as essential criteria to assess a program quality.</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>



.box {
    background-image: url(../assets/img/artist-shape-01-600x577.png), url(../assets/img/maxcoach-shape-13.png), url(../assets/img/maxcoach-shape-14.png);
    background-repeat: no-repeat, no-repeat, no-repeat;
    background-position: -6% 100%, 107% 40%, -50% 100%;
}

// .box {
//     position: relative;
//     overflow-x: hidden;
//     overflow-y: hidden;

//     .artist-shape-1 {
//         position: absolute;
//         transform: rotate(250deg);
//         top: 0;
//         left: -8rem;
//     }

//     .maxcoach-shape-13 {
//         position: absolute;
//         right: -5rem;
//         top: 20%;
//     }

//     .maxcoach-shape-14 {
//         position: absolute;
//         transform: rotate(355deg);
//         top: 0rem;
//         left: -2rem;
//     }
// }
</style>
