<template>
    <span>
      <el-popover
          ref="popover"
          placement="top-start"
          title="{{ $t('characterTitle') }}"
          width="600"
          trigger="hover">
          <el-row>
            <el-col :span="16">
              <div style="padding-right:10px; text-align: justify; word-break: normal;">
                <span>{{ $t('shortDefinition') }}</span>
              </div>
            </el-col>
            <el-col :span="8">
              <el-image style="width: 190px; height: 220px" :src="image" :fit="fit"></el-image>
            </el-col>
          </el-row>
      </el-popover>
      <el-link v-popover:popover type="primary">{{ $t("linkName") }}</el-link>
    </span>
</template>

<script>
  import Vue from 'vue'
  import VueI18n from 'vue-i18n'
  Vue.use(VueI18n)

  export default {
    name: 'Character',
    props: {
      image: String,
      characterData: Object
    },
    beforeMount() {
       var i18n = new VueI18n({locale, characterData})
    },
    data() {
      return {
        locale: process.env.VUE_APP_I18N_LOCALE || 'en'
      };
    },
    methods: {
      
    }
  }
</script>

<style>
</style>
