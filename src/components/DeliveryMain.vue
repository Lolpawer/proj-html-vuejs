<template>
    <div class="delivery-container">
        <div class="container flex wrap">

            <!-- Section title -->
            <div class="delivery-box-title margin-right">
                <p class="teal-text bold">WHAT WE DO</p>
                <p class="section-title-font bold white-text delivery-title">We offer a full range of delivery methods.</p>
                <!-- The green background behind "delivery" -->
                <div class="green-backbox"></div>
            </div>

            <!-- Big delivery box, double the width of 2 smaller boxes (margin included) -->
            <div class="delivery-box-big delivery-background">
                <div class="flex space-between teal-text">
                    <i class="fas fa-shipping-fast"></i>
                    <i class="fas fa-arrow-right arrow"></i>
                </div>
                <p class="white-text bold delivery-subtitle">Shipping Fast</p>
                <p class="silver-text delivery-text">Special fast delivery service that guarantees the arrival of the object on the same day as postage. Included monitoring via mobile app.</p>
            </div>

            <!-- The three smaller delivery boxes -->
            <div class="delivery-box-small delivery-background margin-right">
                <div class="flex space-between teal-text">
                    <i class="fas fa-motorcycle"></i>
                    <i class="fas fa-arrow-right arrow"></i>
                </div>
                <p class="white-text bold delivery-subtitle">Motoboy</p>
                <p class="silver-text delivery-text">Functional motoboy for delivery of documents and small objects.</p>
            </div>

            <div class="delivery-box-small delivery-background margin-right">
                <div class="flex space-between teal-text">
                    <i class="fas fa-shuttle-van"></i>
                    <i class="fas fa-arrow-right arrow"></i>
                </div>
                <p class="white-text bold delivery-subtitle">Shuttle Van</p>
                <p class="silver-text delivery-text">Suitable for medium sized loads that need digital tracking.</p>
            </div>

            <div class="delivery-box-small delivery-background">
                <div class="flex space-between teal-text">
                    <i class="fas fa-truck-moving"></i>
                    <i class="fas fa-arrow-right arrow"></i>
                </div>
                <p class="white-text bold delivery-subtitle">Mini Truck</p>
                <p class="silver-text delivery-text">For dry cargo deliveries with more cubic allocation.</p>
            </div>

        </div>
    </div>
</template>

<script>
</script>

<style lang="scss" scoped>
    .delivery-container {
        background-color: #111117;
        padding: 100px 0;

        .margin-right {
            margin-right: 15px;
        }

        .delivery-background {
            background-color: #19191f;
        }

        .delivery-subtitle {
            font-size: 30px;
            padding: 20px 0;
        }

        .delivery-text {
            font-size: 20px;
        }

        .delivery-box-title {
            width: 390px;
            height: 280px;
            margin-top: 30px;
            position: relative;

            .delivery-title {
                font-size: 50px;
                line-height: 120%;
                padding-top: 20px;
                padding-right: 100px;
                position: absolute;
                z-index: 1;
            }

            .green-backbox {
                width: 220px;
                height: 25px;
                background-color: #058283;
                opacity: 0.5;
                margin-top: 170px;
                margin-left: 60px;
                border-radius: 5px;
            }
           
        }

        .delivery-box-small {
            width: 390px;
            height: 280px;
            margin-top: 30px;
            border-radius: 10px;
            padding: 50px 45px;

        }

        .delivery-box-big {
            width: 795px;
            height: 280px;
            padding: 50px 45px;
            border-radius: 10px;
            margin-top: 30px;

        }

        i {
            font-size: 50px;
        }

        .arrow {
            font-size: 30px;
            opacity: 0.5;
            cursor: pointer;
        }
    }

</style>