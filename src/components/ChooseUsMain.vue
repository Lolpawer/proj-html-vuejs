<template>
    <div class="choose-box">
        <div class="container">
            <div class="relative">
                <div class="section-title-font white-text choose-title absolute">
                    Why choose us?
                </div>
                <div class="green-backbox absolute"></div>
            </div>
            <div class="lightslategray-text choose-text">
                We work intensively in search of ideals that can add up in the lives of our customers. This is what motivates us to improve every day.
            </div>
            <button-green 
            class="button"
            :text="button.contact"/>
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
        button: Object
    }
}
</script>

<style lang="scss" scoped>
    .choose-box {
        background-image: url("../assets/bg-7.jpg");
        background-position: center;
        padding: 290px 0;

        .container {
            text-align: center;

            .relative {
                height: 110px;

                .choose-title {
                    font-weight: bolder;
                    font-size: 70px;
                    z-index: 1;
                    right: 25%;
                    
                }

                .green-backbox {
                    height: 35px;
                    width: 125px;
                    background-color: #058283;
                    opacity: 0.5;
                    top: 50px;
                    right: 300px;
                    border-radius: 5px;
                
                }
            }

            .choose-text {
                font-size: 23px;
                padding: 30px 0;
                margin-bottom: 20px;
            }

            .button {
                margin: 0 auto;
            }
        }
    }

</style>