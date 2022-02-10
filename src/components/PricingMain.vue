<template>
    <div class="pricing-box">
        <div class="container">

            <!-- Title and description of section -->
            <div class="lightseagreen-text bold">MONTHLY PLANS</div>
            <div class="darkslategray-text section-title-font title">Pricing Table</div>
            <div class="lightslategray-text subtext">We can help you deliver and execute your future, wherever you compete, using the latest technologies, from strategy development to implementation.</div>
            
            <!-- Pricing tables -->
            <div class="flex space-between pricing">

                <!-- Leftmost pricing table -->
                <div class="pricing-table">
                    <i class="fas fa-rocket teal-text icon"></i>
                    <p class="darkslategray-text bold pricing-title icon">Standard</p>
                    <p class="teal-text price-text icon">
                        $
                        <span class="price bold">490</span>
                        / mo
                    </p>
                    <ul>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">National Coverage</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Unlimited Motoboy</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Address Collection</p>
                            <i class="fas fa-times teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Mobile App Tracking</p>
                            <i class="fas fa-times teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Cargo Insurance</p>
                            <i class="fas fa-times teal-text"></i>
                        </li>
                    </ul>
                </div>

                <!-- Middle pricing table, taller than the other two and with the "most popular" flair -->
                <div class="pricing-table pricing-middle">
                    <div class="most-popular">Most Popular</div>
                    <i class="fas fa-briefcase teal-text icon"></i>
                    <p class="darkslategray-text bold pricing-title icon">Professional</p>
                    <p class="teal-text price-text icon">
                        $
                        <span class="price bold">890</span>
                        / mo
                    </p>
                    <ul>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">National Coverage</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Unlimited Motoboy</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Address Collection</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Mobile App Tracking</p>
                            <i class="fas fa-times teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Cargo Insurance</p>
                            <i class="fas fa-times teal-text"></i>
                        </li>
                    </ul>
                </div>

                <!-- Rightmost pricing table -->
                <div class="pricing-table">
                    <i class="fas fa-gem teal-text icon"></i>
                    <p class="darkslategray-text bold pricing-title icon">Ultimate</p>
                    <p class="teal-text price-text icon">
                        $
                        <span class="price bold">1.390</span>
                        / mo
                    </p>
                    <ul>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">National Coverage</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Unlimited Motoboy</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Address Collection</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Mobile App Tracking</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                        <li class="flex space-between">
                            <p class="lightslategray-text pricing-text">Cargo Insurance</p>
                            <i class="fas fa-check teal-text"></i>
                        </li>
                    </ul>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
</script>

<style lang="scss" scoped>
    .pricing-box {
        background-color: #eef4ed;
        padding: 100px 0;

        .container {
            margin: 0 auto;
            text-align: center;

            .title {
                font-weight: bolder;
                font-size: 50px;
                padding: 10px 0;
            }

            .subtext {
                font-size: 20px;
                padding: 0 160px;
            }

            .pricing {
                padding: 50px 0;

                .pricing-table {
                    width: 380px;
                    height: 500px;
                    background-color: #fff;
                    padding: 40px 0;
                    margin-top: 10px;
                    border-radius: 10px;

                    .icon {
                        font-size: 45px;
                    }

                    .pricing-title {
                        font-size: 30px;
                        padding: 10px 0;
                    }

                    .price-text {
                        font-size: 20px;

                        .price {
                            font-size: 50px;
                        }
                    }

                    ul {
                        padding: 0 50px;

                        li {
                            padding: 15px 0;
                        }

                        .pricing-text {
                            font-size: 20px;
                        }
                    }
                }

                .pricing-middle {
                    height: 540px;
                    padding: 50px 0;
                    margin-top: 0;
                    position: relative;

                    .most-popular {
                        position: absolute;
                        width: 80px;
                        text-align: start;
                        padding: 10px 10px;
                        background-color: #00a6a6;
                        color: #fff;
                        border-top-right-radius: 25px;
                        border-bottom-right-radius: 25px;
                        top: 12px;
                        font-size: 14px;
                    }
                }
            }
        }
    }

</style>