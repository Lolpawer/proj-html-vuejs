<template>
    <header>
        <div class="company-info">
            <div class="container flex">
                <div class="company-hours">
                    <i class="fas fa-clock"></i>
                    Open Hours: {{days}} - {{hours}}
                </div>
                <div class="contact-information flex">
                    <div>
                        <i class="fas fa-phone"></i>
                        {{number}}
                    </div>
                    <div>
                        <i class="fas fa-envelope"></i>
                        {{email}}
                    </div>
                    <i class="fab fa-facebook-f pointer"></i>
                    <i class="fab fa-twitter pointer"></i>
                    <i class="fab fa-linkedin-in pointer"></i>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    props: {
        days: String,
        hours: String,
        number: String,
        email: String
    }
}
</script>

<style lang="scss" scoped>
    .company-info {
        width: 100%;
        background-color: #21333e;
        color: #c0c3c7;
        font-size: 15px;
        padding: 15px 0;

        .contact-information {
            width: 30%;
        }
    }
       
</style>