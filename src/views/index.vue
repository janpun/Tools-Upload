<template>
  <div class="upload">
    <a-upload draggable directory multiple tip="上传" :headers="headers" :action="action" />
  </div>
</template>
<script setup>
const action = '/'
const headers = ''
</script>
<style lang="scss">
.upload {
  padding: 0 20px;
  padding-top: 10px;
}
</style>
