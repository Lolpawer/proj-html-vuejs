<template>
    <div class="pricing-box">
        <div class="container">
            <div class="lightseagreen-text bold">MONTHLY PLANS</div>
            <div class="darkslategray-text section-title-font title">Pricing Table</div>
            <div class="lightslategray-text subtext">We can help you deliver and execute your future, wherever you compete, using the latest technologies, from strategy development to implementation.</div>
            <div class="flex space-between">

                <div class="pricing-table">
                    <i class="fas fa-rocket teal-text"></i>
                </div>

                <div class="pricing-table">
                    <i class="fas fa-briefcase teal-text"></i>
                </div>

                <div class="pricing-table">
                    <i class="fas fa-gem teal-text"></i>
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

            .pricing-table {
                width: 380px;
                background-color: #fff;
            }
        }
    }

</style>