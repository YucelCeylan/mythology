<template>
    <span>
      <el-popover
          ref="popover"
          placement="top-start"
          title="Gaia / Gaea (Roma: Terra)"
          width="600"
          trigger="hover">
          <el-row>
            <el-col :span="16">
              <div style="padding-right:10px; text-align: justify; word-break: normal;">
                <span>Yeryüzünü, doğayı ve toprağı simgeleyen birinci nesil tanrıdır. Doğa ana ve tüm tanrıların anası olarak
                  görülmüştür. Kaos'un getirdiği düzensizlikten doğarak evrene düzeni getirmiştir. Daha sonra <Uranos/>'u, Dağları 
                  ve Denizi yaratmıştır. Uranos(Gök) ile birleşerek Titanlar'ı, Tepegözler'i ve Hekatonkheir'leri doğurmuştur.</span>
              </div>
            </el-col>
            <el-col :span="8">
              <el-image style="width: 190px; height: 220px" :src="gaiaProfile" :fit="fit"></el-image>
            </el-col>
          </el-row>
      </el-popover>
      <el-link v-popover:popover type="primary">Gaia</el-link>
    </span>
</template>

<script>
  import Uranos from './Uranos';
  export default {
    name: 'Gaia',
    components: { Uranos },
    props: {
    },
    data() {
      return {
        gaiaProfile: require('@/assets/gaia_profile.png'),
      };
    },
    methods: {
    }
  }
</script>

<style>
</style>
