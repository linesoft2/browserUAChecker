<template>
    <div class="block info">
        <span class="left">{{title}}:</span>
        <span class="right">
            <info :content="content.main ? content.main : content"></info>
            <span v-if="content.base">（基于 <info :content="content.base"></info> )</span>
        </span>

    </div>
</template>

<script>
    import info from "./info.vue"
    export default {
        props: ["title", "content"],
        components: {
            info
        }
    }
</script>

<style>
    .info {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .left {
        color: #363636;
        font-size: 1.15rem;
        /* font-weight: 5; */
    }
</style>
