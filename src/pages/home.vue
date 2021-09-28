<template>
    <div id="home" class="tile is-ancestor">
        <div class="tile is-vertical is-parent">
            <div class="box tile is-child">
                <h1 class="title is-5 block box_title">系统</h1>
                 <row title="名称" content=""></row>
                 <row title="版本" content=""></row>
                 <row title="架构" content=""></row>
            </div>
            <div class="box tile is-child">
                <h1 class="title is-5 block box_title">浏览器</h1>
                <row title="名称" content=""></row>
                <row title="版本" content=""></row>
            </div>
        </div>
        <div class="tile is-vertical is-parent">
            <div class="box tile is-child">
                <h1 class="title is-5 block box_title">内核</h1>
                <row title="名称" content=""></row>
                <row title="渲染引擎" content=""></row>
                <row title="JS引擎" content=""></row>
            </div>
            <div class="box tile is-child">
                <h1 class="title is-5 block box_title">原始UA</h1>
                <div>
                    {{ua}}
                </div>
            </div>
        </div>

    </div>
</template>

<script>
    import row from '../components/row.vue'
    export default {
        data(){
            return{
                ua: navigator.userAgent
            }
        },
        components: {
            row
        },
        created(){
            // const ua = this.ua = navigator.userAgent
            // console.log("test")
        },
        computed:{
            // system(){
                // const ua = this.ua
                // const result = {name:{},abi:""}
                
                // return result
            // }
            
        }
    }
</script>

<style>
    .box_title {
        padding-bottom: 0.625rem;
        border-bottom: 0.125rem solid #f5f5f5;
    }
</style>
