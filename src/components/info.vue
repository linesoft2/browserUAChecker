<template>
    <span id="info">
        <img v-if="content.img" src="content.img">
        <span>{{content.name ? content.name : content}}</span>
    </span>
</template>

<script>
    export default {
        props:["content"]
    }
</script>

<style>
</style>
