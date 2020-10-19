<template>
    <span>
      <el-popover
          ref="popover"
          placement="top-start"
          title= "{{$t('shortDefinition')}}"
          width="600"
          trigger="hover">
          <el-row>
            <el-col :span="16">
              <div style="padding-right:10px; text-align: justify; word-break: normal;">
                <span>{{ $t('shortDefinition') }}</span>
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
  export default {
    name: 'Gaia',
    props: {
    },
    data() {
      return {
        gaiaProfile: require('@/assets/gaia_profile.png'),
        characterData: {
          tr: {
            name: "Gaia / Gaea (Roma: Terra)",
            link: "Gaia",
            shortDefinition: "Yeryüzünü, doğayı ve toprağı simgeleyen birinci nesil tanrıdır. Doğa ana ve tüm tanrıların anası olarak görülmüştür. Kaos'un getirdiği düzensizlikten doğarak evrene düzeni getirmiştir. Daha sonra Uranos'u, Dağları ve Denizi yaratmıştır. Uranos (Gök) ile birleşerek Titanlar'ı, Tepegözler'i ve Hekatonkheir'leri doğurmuştur."
          },

          en: {
            name: "Gaia / Gaea (Roman: Terra)",
            link: "Gaia",
            shortDefinition: "She is the first generation god who symbolizes the earth and nature. She was seen as mother nature and the mother of all gods. She brought order to the universe, arising from the disorder brought about by chaos. Shee later created Uranos, Mountains and Sea. Merged with Uranos (Sky) to give birth to the Titans, Cyclopes and Hekatonkheirs."
          }
        }
      };
    },
    methods: {
    }
  }
</script>

<style>
</style>
