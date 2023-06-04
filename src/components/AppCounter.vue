<script >
import ButtonCustom from './ButtonCustom.vue';

export default {
    nome: "AppCounter",
    components: {
        ButtonCustom,
    }
}
</script>

<template>
    <div class="d-flex justify-content-center align-items-center p-2">
        <p class="text-secondary-emphasis m-0 pe-4">Starts TOMORROW! Our biggest event of the year...</p>
        
        <div class="fw-bold pe-4">
            <span class="pe-2 fs-5">
                <i class="fa-solid fa-stopwatch"></i>
            </span>
            <span>
                00 : 00 : 00
            </span>
        </div>
        
        <ButtonCustom class="text-white" text="Get ticket" />
    </div>
</template>

<style lang="scss" scoped>
@use '../variables.scss' as *;

    div {
        background-color: $LightGray;
    }

    button{
        background-color: $Primary;

        &:hover{
            background-color: $Sky;
        }
    }
</style>
