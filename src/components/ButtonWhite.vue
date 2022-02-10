<template>
    <div class="lightseagreen-text pointer">
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
        border: 1px solid #00a6a6;
        font-weight: bold;
        border-radius: 5px;
        text-align: center;
        line-height: 46px;
    }

</style>