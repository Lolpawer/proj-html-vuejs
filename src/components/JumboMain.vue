<template>
    <div class="jumbotron darkslategray-text">

        <!-- Navbar in the Jumbotron, alongside the logo -->
        <div class="container flex space-between">

            <!-- Logo -->
            <div class="logo">
                <img src="../assets/logo.svg" />
            </div>

            <!-- Navbar -->
            <nav>
                <ul class="flex space-between">
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

        <!-- Jumbotron content -->
            <div class="container">
                <div class="jumbotron-content">
                    <div class="lightseagreen-text bold">
                        EXPRESS DELIVERY
                    </div>
                    <div class="jumbotron-text section-title-font darkslategray-text">
                        What are we going to deliver 
                        <span class="teal-text">today?</span>
                        <!-- The little green background behind "today?" -->
                        <div class="green-backbox">
                        </div>
                    </div>
                    <div class="flex button-row">
                        <button-green
                        class="jumbo-button"
                        :text="button.contact" />
                        <button-white
                        class="jumbo-button"
                        :text="button.information" />
                    </div>
                </div>
            </div>


    </div>
</template>

<script>
import ButtonGreen from './ButtonGreen.vue'
import ButtonWhite from './ButtonWhite.vue'

export default {
    components: {
        ButtonGreen,
        ButtonWhite
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

        .jumbotron-content {
            width: 50%;
            padding-top: 150px;

            .jumbotron-text {
                font-weight: bolder;
                font-size: 70px;
                z-index: 1;
                line-height: 130%;

                .green-backbox {
                    background-color: #cbe4de;
                    width: 255px;
                    height: 38px;
                    margin-top: -45px;
                    border-radius: 5px;
                }
            }

            .button-row {
                padding-top: 50px;

                .jumbo-button {
                    margin-right: 30px;

                }
            }
        }
    }

</style>