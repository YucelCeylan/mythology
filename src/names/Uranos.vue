<template>
    <span>
      <el-popover
          ref="popover"
          placement="top-start"
          title="Uranos"
          width="200"
          trigger="hover"
          content="Gökyüzü ve evreni simgeleyen birinci nesil tanrıdır. Gaia tarafından yaratılmıştır. 
        12 titanın, hekatheironların ve tepegözlerin babasıdır...">
      </el-popover>
      <el-link v-popover:popover type="success" icon="fas fa-mars">Uranos</el-link>
    </span>
</template>

<script>
  export default {
    name: 'Uranos',
    props: {
    },
    data() {
      return {
        
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
