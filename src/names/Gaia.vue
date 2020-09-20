<template>
    <span>
      <el-popover
          ref="popover"
          placement="top-start"
          title="Gaia"
          width="200"
          trigger="hover"
          content="Doğayı, toprağı ve düzeni simgeleyen birinci nesil tanrıdır. Titanların, hekatheironların ve tepegözlerin annesidir.
          Aynı zamanda kocası olan Uranus'u da o yaratmıştır.">
      </el-popover>
      <el-link v-popover:popover type="success" icon="fas fa-venus">Gaia</el-link>
    </span>
</template>

<script>
  export default {
    name: 'Gaia',
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
</style>
