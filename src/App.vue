<template>
  <header>
    <div class="wrapper">
      <nav>
        <!-- <router-link to="/">首页</router-link>
        <router-link to="/pins">沸点</router-link>
        <router-link to="/news">资讯</router-link>
        <router-link to="/course">课程</router-link>
        <router-link to="/events/all">活动</router-link> -->
        <HeaderComponentVue/>
      </nav>
    </div>
  </header>
  <router-view />
</template>

<script setup lang="ts">
  import HeaderComponentVue from '@components/HeaderComponent/index.vue';
</script>

