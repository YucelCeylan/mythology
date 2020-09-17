<template>
  <div>
    <el-row id="history">
        <el-col :span="10">
            <el-timeline>
                <el-timeline-item v-for="(activity, index) in activities" :key="index" :timestamp="activity.timestamp">
                    <el-button type="info" icon="el-icon-d-arrow-right">{{activity.content}}</el-button>
                </el-timeline-item>
            </el-timeline>
        </el-col>
        <el-col id="history_description" :span="14">
            <span> 
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
            </span>
        </el-col>
    </el-row>
  </div>
</template>

<script>
  export default {
    name: 'history',
    props: {
    },
    data() {
      return {
        activities: [
            {
              content: "Baslik 1",
              timestamp: 'M.Ö. 20000'
            },
            {
              content: "Baslik 2",
              timestamp: 'M.Ö. 10000'
            },
            {
              content: "Baslik 3",
              timestamp: 'M.Ö. 10000'
            },
            {
              content: "Baslik 4",
              timestamp: 'M.Ö. 10000'
            }
        ]
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
