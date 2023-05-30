<script >


export default {
    components: {
        nome: "AppCounter"
    }
}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center p-2">
        <p class="text-secondary-emphasis m-0 pe-4">Starts TOMORROW! Our biggest event of the year...</p>
        <div class="fw-bold">
            <span class="pe-2 fs-5">
                <i class="fa-solid fa-stopwatch"></i>
            </span>
            <span>
                00 : 00 : 00
            </span>
        </div>
        <button class="btn text-white ms-4 px-5 fw-bold">Get ticket</button>
    </div>
</template>

<style lang="scss" scoped>

$LightGray: #F5F5F5;
$Orange: #Ef6F31;

    div {
        background-color: $LightGray;
    }

    button{
        background-color: $Orange;

        &:hover{
            background-color: red;
        }
    }
</style>
