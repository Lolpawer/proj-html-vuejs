<template>
    <div class="box">
        <div class="container flex">

            <div class="form-box">
                <div class="lightseagreen-text bold">
                    SEND A MESSAGE
                </div>
                <div class="darkslategray-text section-title-font get-in-touch-title">
                    Get in
                    <span class="touch teal-text">
                        Touch
                    </span>
                </div>
                <div class="lightslategray-text">
                    We will respond to your message as soon as possible.
                </div>
                <form> 
                    <input type="text" placeholder="Name">
                    <input type="email" placeholder="Email">
                    <input type="number" placeholder="Phone">
                    <select>
                        <option selected hidden>More Info</option>
                        <option>Actually there is nothing here</option>
                        <option>Sorry</option>
                    </select>
                    <textarea placeholder="Message" rows="5"></textarea>
                </form>
                <button-green 
                :text="button.send"/>
            </div>

            <div class="company-box">
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
    .box {
        padding: 100px 0;

        .lightslategray-text {
            font-size: 20px;

        }

        .form-box {
            width: 70%;

            .get-in-touch-title {
                font-size: 50px;
                font-weight: bolder;
                padding: 20px 0;

                .touch{
                    background-color: #daeced;
                    padding: 0 20px;
                    border-radius: 5px;

                }
            }

            form {
                padding-top: 50px;

                * {
                    width: 45%;
                    margin-right: 5%;
                    margin-bottom: 20px;
                    background-color: #ececec;
                    border: solid 1px #ececec;
                    border-radius: 5px;
                    font-size: 20px;
                    padding: 15px 10px;

                    &::placeholder {
                        color: #829397;
                    }
                }

                select {
                    color: #829397;

                    option {
                        color: #000;

                    }
                }

                textarea {
                    width: 95%;
                }
            }
        }

        .company-box {
            width: 30%;
        }
    }

</style>