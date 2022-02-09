<template>
    <div class="jumbotron darkslategray-text">

        <!-- Navbar in the Jumbotron, alongside the logo -->
        <div class="container flex">

            <!-- Logo -->
            <div class="logo">
                <img src="../assets/logo.svg" />
            </div>

            <!-- Navbar -->
            <nav>
                <ul class="flex">
                    <li 
                    class="pointer"
                    v-for="(object, index) in nav"
                    :key="index">
                    {{object.text}}
                    </li>
                    <li><i class="far fa-user pointer"></i></li>
                    <li>
                        <button-green
                        :text="button.contact"/>
                    </li>
                </ul>
            </nav>

        </div>

    </div>
</template>

<script>
import ButtonGreen from './ButtonGreen.vue'

export default {
    components: {
        ButtonGreen
    },
    props: {
        nav: Array,
        button: Object
    }
}
</script>

<style lang="scss" scoped>
    .jumbotron {
        padding: 15px 0;
        background-image: url("../assets/bg-13.jpg");
        background-position: center;
        height: 860px;

        .logo {
            width: 120px;
        }

        nav {
            line-height: 46px;
            width: 55%;

            ul {
                list-style: none;

                li {
                    padding: 0 5px;
                }
            }
        }
    }

</style>