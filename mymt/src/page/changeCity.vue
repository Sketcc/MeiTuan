<template>
  <div class="page-changeCity">
    <el-row>
      <province />
    </el-row>
    <el-row>
      <hot title="热门城市 :" :list="hotList" />
    </el-row>
    <el-row>
      <hot title="最近访问 :" :list="rencentList" />
    </el-row>
    <el-row>
        <categroy />
    </el-row>
  </div>
</template>

<script>
import Province from "@/components/changeCity/province.vue";
import hot from "@/components/changecity/hot.vue";
import Categroy from  "@/components/changecity/category.vue"
export default {
    data() {
        return {
            hotList:["哈尔滨", "佳木斯", "牡丹江", "鹤岗"],
            rencentList:["哈尔滨", "佳木斯", "牡丹江", "鹤岗"]
        }
    },
  components: {
    Province,
    hot,
    Categroy
  }
};
</script>

<style lang="scss">
   @import "@/assets/css/changecity/hot.scss"
</style>