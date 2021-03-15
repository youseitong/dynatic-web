<template>
  <el-input v-model="input" placeholder="请输入内容"></el-input>
</template>

<script>
export default {
  props: {
    input: {
      type: String,
      default: "",
    },
  },
  watch: {
    input(val) {
      this.$emit("update:input", val);
    },
  },
};
</script>

<style></style>
