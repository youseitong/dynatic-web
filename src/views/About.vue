<template>
  <div>
    <component
      :is="com"
      v-for="(com, index) in comList"
      :input.sync="input[index]"
      :key="index"
      @click="click()"
    ></component>
  </div>
</template>

<script>
export default {
  components: {
    Input: () => import("../components/Input"),
    Select: () => import("../components/Select"),
    Button: () => import("../components/Button"),
  },
  created() {},
  data() {
    return {
      comList: ["Input", "Select", "Button"],
      input:['12','444']
    };
  },
  methods: {
    click() {
      console.log(123,this.input);
    },
  },
};
</script>

<style></style>
