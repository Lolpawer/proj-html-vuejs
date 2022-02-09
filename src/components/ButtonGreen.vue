<template>
    <div class="linen-text pointer">
        {{text}}
    </div>
</template>

<script>
export default {
    props: {
        text: String
    }
}
</script>

<style lang="scss" scoped>
    div {
        height: 46px;
        width: 160px;
        background-color: #058283;
        font-weight: bold;
        border-radius: 5px;
        text-align: center;
        vertical-align: middle;
    }

</style>