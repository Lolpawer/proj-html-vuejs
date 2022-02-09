<template>
    
    <div class="leaders-box">
        <div class="container leaders-container flex">
            <div class="leaders-content">
                <div class="lightseagreen-text bold">
                    WHO WE ARE
                </div>
                <div class="leaders-big-text section-title-font darkslategray-text">
                    Industry Leaders.
                </div>
                <div class="leaders-text lightslategray-text">
                    With all of this expertise and capability comes an unrivaled commitment to customer service.
                </div>
                <div class="leaders-text lightslategray-text">
                    We will work hard to understand your needs in order to develop a productive, long-term partnership.
                </div>
                <button-green 
                class="button"
                :text="button.information"/>
            </div>
        </div>
    </div>
</template>

<script>
import ButtonGreen from './ButtonGreen.vue';

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
    .leaders-box {
        background-image: url("../assets/bg-6.jpg");
        height: 860px;
        background-position: center;

        .leaders-container {
            justify-content: flex-end;

            .leaders-content {
                width: 45%;
                padding-top: 150px;

                .leaders-big-text {
                    font-weight: bolder;
                    font-size: 70px;
                    z-index: 1;
                    line-height: 130%;
                }

                .leaders-text {
                    font-size: 23px;
                    padding: 20px 0;
                }

                .button {
                    margin-top: 30px;
                }
            }
        }
    }
        
    
    

</style>