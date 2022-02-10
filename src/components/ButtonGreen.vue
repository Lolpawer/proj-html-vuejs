<!-- MULTI PURPOSE BUTTON WITH GREEN BACKGROUND AND WHITE TEXT -->
<!-- THE BUTTON CONTENT IS DYNAMIC, IN APP LOOK FOR "buttonContent" ARRAY IN DATA -->
<!-- THE MAIN CONTENTS ARE THIS: contact: "GET IN TOUCH",
                                 information: "READ MORE",
                                 send: "SEND",
                                 location: "VIEW MAP" -->
<!-- BIND ONE OF THESE WHEN CREATING A BUTTON WITH :text="button.(text you want displayed)"-->

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
        line-height: 46px;
    }

</style>