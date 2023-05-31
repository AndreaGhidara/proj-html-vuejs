<script >
import ButtonCustom from './ButtonCustom.vue';

export default {
    nome: "AppCoachingNote",
    components: {
        ButtonCustom
    }
}
</script>

<template>
    <div>
        <div class="container">
            <div class="row">
                <div class="col py-5 text-center d-flex flex-column align-items-center">
                    <img src="../assets/img/artist-quote-icon.png" alt="">
                    <div class="pt-3">
                        <h1 class="fw-bold">I coach and mentor <br> visual artist, like <br> you, to Create Like <br> You Mean It</h1>
                        <h2 class="artist">Martin Garrix</h2>
                    </div>
                </div>
                <div class="col py-5">
                    <p class="pt-5">
                        As a coach and mentor, my ultimate goal is to motivate visual artists
                        toward inspired action. I help you get you back on track to being the
                        productive, creative, meaningful and authentic artist you truly want
                        to bel support artists in crafting and living a creative life as well as
                        feeling good about themselves and their art.
                        <br>
                        <br>
                        As an artist and an educator for nearly 30 years, I understand what it
                        takes to create.
                    </p>
                    <ButtonCustom class="px-5" text="Get started today" />
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
$Orange: #Ef6F31;
$Sky: #6AC5F1;

button {
    color: $Orange;
    background-color: #fdf0ea;

    &:hover {
        background-color: $Sky;
    }
}

</style>
