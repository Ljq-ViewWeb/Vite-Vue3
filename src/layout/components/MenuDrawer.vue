<template>
  <el-drawer
    v-model="showMenu"
    title="I am the title"
    :with-header="false"
    :before-close="closeDrawer"
    direction="ltr"
  >
    <span>Hi there!</span>
  </el-drawer>
</template>

<script>
export default {
  name: "MenuDrawer",
  props: {
    showMenu: {
      type: Boolean,
    },
  },
  methods: {
    closeDrawer() {
      this.$emit("update:showMenu", false);
    },
  },
};
</script>

<style>
</style>