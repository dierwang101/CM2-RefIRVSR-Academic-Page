<script lang="ts" setup>
// 页脚需要的链接
const links = {
    Nerfies: "https://github.com/nerfies/nerfies.github.io",
    Vue: "https://cn.vuejs.org/",
    Vite: "https://cn.vitejs.dev/",
    ElementPlus: "https://element-plus.org/zh-CN/",
    template: "https://github.com/JunyaoHu/academic-project-page-template-vue",
}
</script>

<template>
  
  <div class="bg">
    
    <el-watermark :content="['JunyaoHu', 'Academic Project', 'Page Template']" :gap="['60','0']" :z-index="0">
      <el-row justify="center">
        <p class="footer">
          This template is inspired by 
          <a :href="links.Nerfies">Nerfies</a>,<br/>
          
          powered by 
          <a :href="links.Vue">Vue</a>, 
          <a :href="links.Vite">Vite</a>, and
          <a :href="links.ElementPlus">Element Plus</a>.<br/>
          
          You can fork🛠️ / star✨/ PR📃 from <a :href="links.template">here</a>.
        </p>
      </el-row>
    </el-watermark>
  </div>
</template>

<style scoped>

/* 页脚背景 */
.bg {
  background-color: rgba(245, 245, 245, 0.5);
}

/* 页脚文字 - 调整为更不显眼的样式 */
.footer {
  text-align: center;
  margin: 1px 0;
  font-size: 8px;
  color: #aaa;
  z-index: 1;
  line-height: 1;
  opacity: 0.6;
}

</style>
