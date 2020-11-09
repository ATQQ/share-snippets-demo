<template>
    <div class='index'>
      <my-input type='text' clearable :disabled='false' size='small' :labelWidth='120' placeholder='请输入名称' />
    </div>
</template>

<script lang='ts'>
import { defineComponent, reactive, ref, onMounted, computed } from '@vue/composition-api'
export default defineComponent({
  name: 'index',
  setup(_, context) {
    console.log()
    return {}
  },
  components: {},
})
</script>
<style lang='less' scoped>

</style>