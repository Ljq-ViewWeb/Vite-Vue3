<template>
  <el-container style="height:100%">
    <el-header style="background: linear-gradient(to right, #1890ff, #33ffff);height:40px">
      <hello-header></hello-header>
    </el-header>
    <el-main>
      <el-card style="height:100%" body-style="height:100%">
        <router-view />
      </el-card>
    </el-main>
  </el-container>
</template>

<script lang="ts">
import HelloHeader from "./HelloHeader.vue";
export default {
  name: "layout",
  components: { HelloHeader },
};
</script>

<style>
</style>