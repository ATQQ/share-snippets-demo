<template>
    <div class='index.vue'>
      <my-form v-model='formData' ref='myForm'>
        <my-input label='姓名' :labelWidth='120' placeholder='请输入名称' helper='常驻辅助信息' type='email' :readonly='true' clearable />
      </my-form>
    </div>
</template>

<script lang='ts'>
import { defineComponent, reactive, ref, onMounted } from '@vue/composition-api'
export default defineComponent({
  name: 'index.vue',
  setup(_, context) {
    return {}
  },
  components: {},
})
</script>
<style lang='less' scoped>

</style>