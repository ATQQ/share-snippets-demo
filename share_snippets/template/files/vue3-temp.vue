<template>
    <div class='index'>
      <my-input label='姓名' :labelWidth='120' placeholder='请输入名称' />
    </div>
</template>

<script lang='ts'>
import { defineComponent, reactive, ref, onMounted } from '@vue/composition-api'

export default defineComponent({
  name: 'index',
  setup(_, context) {

    return {}
  },
  components: {},
})
</script>
<style lang='less' scoped>

</style>