<template>
  <div>
    <el-row id="headers">
        <el-col :span="12" style="padding-top: 20px; background: #282c25;">
            Titanlar, Uranos ve Gaia'dan doğan ikinci nesil tanrılardır. 6 erkek, 6 dişi olmak üzere toplam 12 titan vardır.
        </el-col>
        <el-col :span="12" style="padding-top: 20px; background: #282c25;">
            Temsili
        </el-col>
    </el-row>
    <el-row id="titans">
        <el-col :span="12" style="padding: 20px; background: #282c25;">
            <el-collapse accordion>
                <el-collapse-item name="1">
                    <template slot="title">
                        <i class="fas fa-mars"></i>Kronos
                    </template>
                    <div>Uranos ve Gaia'nın en küçük oğludur. Zamana hükmeden titandır. Babası Uranos'un hükmüne son vererek onu Tartaros'a hapsetmiştir.</div>
                </el-collapse-item>
                <el-collapse-item name="2">
                    <template slot="title">
                        <i class="fas fa-mars"></i> Hyperion
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="3">
                    <template slot="title">
                        <i class="fas fa-mars"></i> Okeanos
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="4">
                    <template slot="title">
                        <i class="fas fa-mars"></i> Koios
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="5">
                    <template slot="title">
                        <i class="fas fa-mars"></i> Krios
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="6">
                    <template slot="title">
                        <i class="fas fa-mars"></i> İapetos
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="7">
                    <template slot="title">
                        <i class="fas fa-venus"></i> Theia
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="8">
                    <template slot="title">
                        <i class="fas fa-venus"></i> Rheia
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="9">
                    <template slot="title">
                        <i class="fas fa-venus"></i> Themis
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="10">
                    <template slot="title">
                        <i class="fas fa-venus"></i> Phoibe
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="11">
                    <template slot="title">
                        <i class="fas fa-venus"></i> Mnenosyne
                    </template>
                    <div></div>
                </el-collapse-item>
                <el-collapse-item name="12">
                    <template slot="title">
                        <i class="fas fa-venus"></i> Tethys
                    </template>
                    <div></div>
                </el-collapse-item>
            </el-collapse>
        </el-col>
        <el-col :span="12" style="padding: 20px; background: #282c25;">

        </el-col>
    </el-row>
  </div>
</template>

<script>
  export default {
    name: 'titans',
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
    .el-collapse-item__content {
        font-size: 17px !important;
        color: white !important;
        font-style: italic;
        background-color: #282c25;
    }
    .el-collapse-item__header {
        font-size: 17px !important;
        padding-left: 5px;
        color: #00a4af !important;
        background-color: #282c25 !important;
    }
</style>
