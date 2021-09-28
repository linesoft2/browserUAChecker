<template>
    <div id="app">
        <b-navbar class="header" :shadow="true" :mobile-burger="false">
            <template v-slot:brand>
                <b-navbar-item tag="div" class="title_">
                    浏览器运行环境展示
                </b-navbar-item>
            </template>

        </b-navbar>
        <home class="container_"></home>
        <footer class="footer">
            <div class="content has-text-centered">
                <p>
                    本页面所显示的信息基于浏览器的UA（用户代理，User-Agent）得出，该数据可被浏览器/用户等修改，不保证准确性。
                    <br>
                    By 双霖（LineSoft）
                </p>
            </div>
        </footer>
    </div>
</template>

<script>
    import home from './pages/home.vue'

    export default {
        name: 'App',
        components: {
            home
        }
    }
</script>

<style>
    #app {
        /* text-align: center; */
    }

    .header {
        display: flex;
        align-items: center;
        justify-content: center;
        margin-bottom: 1.25rem;
    }

    .title_ {
        width: 100%;
        text-align: center;
        display: flex;
        align-items: center;
        justify-content: center;

    }

    .navbar-menu {
        flex-grow: unset !important;
    }

    .container_ {
        margin-left: 1.25rem !important;
        margin-right: 1.25rem !important;
    }
</style>
