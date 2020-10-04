<template>
  <div>
    <div class="block" :span="24">
      <el-image style="width: %100; height: 100%" fit="none" :src="masterTopJpg" ></el-image>
      <el-menu :default-active="activeIndex" class="main_menu" mode="horizontal" @select="changeTab" background-color="black" text-color = "#fff" active-text-color = "#00a81c">
        <el-menu-item index="1">Genel</el-menu-item>
        <el-menu-item index="2">Titanlar</el-menu-item>
        <el-menu-item index="3">Olimpos Tanrıları</el-menu-item>
        <el-menu-item index="4">Yarı Tanrılar</el-menu-item>
        <el-menu-item index="5">Kahramanlar</el-menu-item>
        <el-menu-item index="6">Hikayeler</el-menu-item>
      </el-menu>
    </div>
    <div>
      <general v-if="activeIndex == '1'"/>
      <titans v-if="activeIndex == '2'"/>
      <history v-if="activeIndex == '6'"/>
    </div>
  </div>
</template>

<script>
  import History from './History.vue';
  import Titans from './Titans.vue';
  import General from './General.vue';

  export default {
    name: 'master',

    components: { History, Titans, General },

    props: {
    },

    data() {
      return {
        masterTopJpg: require('@/assets/master_top.jpg'),
        activeIndex: '1'
      };
    },

    methods: {
      changeTab(key) {
        this.activeIndex = key;
      }
    }
  }
</script>

<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 150px;
    margin: 0;
  }

  .el-carousel__item:nth-child(2n) {
    background-color: #99bf9f;
  }

  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }

  .el-carousel__indicators--outside button {
    background-color: #00a81c !important;
  }

  /* .block {
    position: fixed;
    top:10;
    left: 10;
  } */
</style>
