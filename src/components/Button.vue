<template>
  <el-button type="primary" @click="click">主要按钮</el-button>
</template>

<script>
export default {
  methods: {
    click() {
      console.log("inside");
      this.$emit("click");
    },
  },
};
</script>

<style></style>
