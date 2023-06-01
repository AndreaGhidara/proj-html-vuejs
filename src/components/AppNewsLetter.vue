<script>

export default {
    nome: "AppNewsLetter",
    components: {

    },
    data(){
        return {
            exploreLink: [
                "start here",
                "success story",
                "Blog",
                "Courses",
                "Contact us"
            ],
            InformationLink: [
                "Membership",
                "Purchase guide",
                "Privacy policy",
                "Terms of services"
            ],
        }
    },
    methods:{

    }
    
}
</script>

<template>
    <div class="boxed d-flex my-4">
        <div class="container d-flex align-items-center text-white ">
            <h2 class="pe-5 ps-5  fs-2 text-end">
                Newsletter to get <br>
                in touch
            </h2>

            <div class="test d-flex align-items-center ms-5 h-25 w-50">
                <form class="w-100 d-flex align-items-center" action="#">
                    <input class="text-white text-decoration-none" placeholder="Your e-mail" type="mail">
                    <div class="send">
                        <i class="fa-solid fa-arrow-right-long"></i>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
$Blu: #244186;

::placeholder {
    /* Chrome, Firefox, Opera, Safari 10.1+ */
    color: #fff;
    opacity: 1;
    /* Firefox */
}

:-ms-input-placeholder {
    /* Internet Explorer 10-11 */
    color: #fff;
}

::-ms-input-placeholder {
    /* Microsoft Edge */
    color: #fff;
}

input {
    background-color: transparent;
    border: none;
    outline: none;
    width: 100%;
}

.boxed {
    height: 200px;
    background-color: $Blu;
    background-image: url(../assets/img/artist-shape-color-paint-bottom-right.png), url(../assets/img/artist-shape-color-paint-top-left.png);
    background-repeat: no-repeat, no-repeat;
    background-position: 100% 100%, -0% 0%;

    .send {
    cursor: pointer;
    }
}

.test {
    margin: 0;
    padding: 0;
    border-bottom: 1px solid rgb(255, 253, 253);
}
</style>
