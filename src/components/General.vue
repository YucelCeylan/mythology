<template>
  <div style="padding-top:20px">
    <el-timeline>
      <el-timeline-item key="1">
        <el-container>
          <el-aside width="310px">
            <el-avatar shape="circle" :size="300" :fit="fit" :src="khaosProfile"></el-avatar>
          </el-aside>
          <el-main>
            <el-container>
              <el-header>Khaos</el-header>
              <el-main>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
                et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip 
                ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu 
                fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt 
                mollit anim id est laborum.
              </el-main>
            </el-container>
          </el-main>
        </el-container>
      </el-timeline-item>
      <el-timeline-item key="2" size="large" placement="bottom">
        <el-container>
          <el-aside width="310px">
            <el-avatar shape="circle" :size="300" :fit="fit" :src="gaiaProfile"></el-avatar>
          </el-aside>
          <el-main>
            <el-container>
              <el-header>Gaia</el-header>
              <el-main>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
                et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip 
                ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu 
                fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt 
                mollit anim id est laborum.
              </el-main>
            </el-container>
          </el-main>
        </el-container>
      </el-timeline-item>
      <el-timeline-item key="3" size="large" placement="bottom">
        <el-container>
          <el-aside width="310px">
            <el-avatar shape="circle" :size="300" :fit="fit" :src="uranosProfile"></el-avatar>
          </el-aside>
          <el-main>
            <el-container>
              <el-header>Uranos</el-header>
              <el-main>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore 
                et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip 
                ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu 
                fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt 
                mollit anim id est laborum.
              </el-main>
            </el-container>
          </el-main>
        </el-container>
      </el-timeline-item>
    </el-timeline>
  </div>
</template>

<script>
  export default {
    name: 'general',
    props: {
    },
    data() {
      return {
        khaosProfile: require('@/assets/khaos_profile2.png'),
        gaiaProfile: require('@/assets/gaia_profile2.png'),
        uranosProfile: require('@/assets/uranos_profile2.png'),
      };
    },
    methods: {
    }
  }
</script>

<style>
    #history {
      background: #282c25;
      padding-top: 30px;
    }
    #history_description {
      position: fixed;
      text-align: left;
      left:550px;
      top:270px;
    }
    .el-timeline-item__content {
      color: #00a81c;
    }
    .el-timeline-item__wrapper {
      text-align: left;
    }
</style>
