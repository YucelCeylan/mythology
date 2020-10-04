<template>
    <span>
      <el-popover
          ref="popover"
          placement="top-start"
          title="Uranos / Uranüs (Roma: Caelus / Coelus)"
          width="600"
          trigger="hover"
          content="">
          <el-row>
            <el-col :span="16">
              <div style="padding-right:10px; text-align: justify; word-break: normal;">
                <span>
                    Gökyüzü ve uzayı simgeleyen birinci nesil tanrıdır. Gaia tarafından yaratılmıştır. Aynı zamanda Gaia'nın 
                    kocası ve tanrıların babası olarak bilinmektedir. Titanlar'ın, Tepegözler'in ve Hekatonkheir'lerin babasıdır.
                </span>
              </div>
            </el-col>
            <el-col :span="8">
              <el-image style="width: 190px; height: 220px" :src="uranosProfile" :fit="fit"></el-image>
            </el-col>
          </el-row>
      </el-popover>
      <el-link v-popover:popover type="primary">Uranos</el-link>
    </span>
</template>

<script>
  export default {
    name: 'Uranos',
    props: {
    },
    data() {
      return {
        uranosProfile: require('@/assets/uranos_profile.png'),
      };
    },
    methods: {
    }
  }
</script>

<style>
  .el-link.el-link--success {
    font-size: 17px !important;
  }
</style>
