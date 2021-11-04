<template>
  <div>
    <!-- <input type="text" v-model="nameComputed" placeholder="输入字母会自动转换成大写" /> -->
    <el-input type="text" placeholder 
    
    
    v-model="service" 
    v-mask="serviceNameMask" 
    
    clearable></el-input>
    {{show}}
  </div>
</template>

<script>
import { mask } from "vue-the-mask";

export default {
  data() {
    return {
      name: "",
      service: "",
      serviceNameMask: {
        mask: "AAAA-AAAA-AAAA-AAAA",
        tokens: {
          A: {
            pattern: /[0-9a-zA-Z]/,
            transform: (v) => v.toLocaleUpperCase(),
          },
        },
      },
    };
  },
  directives: { mask },
  methods: {},
  computed: {
    show() {
      return this.service.replace(/-/g, '');
    },
  },
};
</script>

<style lang="scss" scoped>
</style>