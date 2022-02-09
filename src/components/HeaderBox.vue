<template>
    <!-- Header where all the info and socials are -->
    <header class="silver-text">
        <div class="container flex space-between">

            <!-- Opening hours -->
            <div>
                <i class="fas fa-clock"></i>
                Open Hours: {{companyInfo.days}} - {{companyInfo.hours}}
            </div>

            <!-- Phone number, email and socials -->
            <div class="contact-information flex space-between">
                <div>
                    <i class="fas fa-phone"></i>
                    {{companyInfo.phoneNumber}}
                </div>
                <div>
                    <i class="fas fa-envelope"></i>
                    {{companyInfo.email}}
                </div>
                <div><i class="fab fa-facebook-f pointer"></i></div>
                <div><i class="fab fa-twitter pointer"></i></div>
                <div><i class="fab fa-linkedin-in pointer"></i></div>
            </div>

        </div>
    </header>
</template>

<script>
export default {
    props: {
        companyInfo: Object
    }
}
</script>

<style lang="scss" scoped>
    header {
        width: 100%;
        background-color: #21333e;
        font-size: 15px;
        padding: 15px 0;

        .contact-information {
            width: 40%;
        }

    }
</style>