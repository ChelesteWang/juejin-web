<template>
    <div>
        <router-link to="/">
            <img :src="logoUrl.desktop" class="logo-img" alt="稀土掘金" />
            <img :src="logoUrl.mobiles" class="logo-img" alt="稀土掘金" />
            <img
                src="https://p6-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/e04bb958a0204f37b648e7883cfb158a~tplv-k3u1fbpfcp-zoom-1.image"
                alt="人气创作者榜单"
                style="width: 150px; vertical-align: -11px;"
            />
        </router-link>
    </div>
    <div v-for="route in routes">
        <router-link :to="route.url">{{ route.msg }}</router-link>
    </div>
</template>

<script setup lang="ts" >
const logoUrl = {
    desktop: '//lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/7abc2b532f725d394feaf0141547ade7.svg',
    mobiles: '//lf3-cdn-tos.bytescm.com/obj/static/xitu_juejin_web/6bdafd801c878b10edb5fed5d00969e9.svg'
}
const routes = [
    {
        url: '/',
        msg: '首页'
    },
    {
        url: '/pins',
        msg: '沸点'
    },
    {
        url: '/news',
        msg: '资讯'
    },
    {
        url: '/course',
        msg: '课程'
    },
    {
        url: '/events/all',
        msg: '活动'
    }
];
</script>

<style scoped>
.logo-img {
    display: block;
    width: 116.82px;
    height: 24px;
}
</style>