<template>
    <div class='demo.vue'>
        <my-button type1='value2' type2='value2'></my-button>
    </div>
</template>

<script lang='ts'>
import { defineComponent, reactive, ref, onMounted } from '@vue/composition-api'

export default defineComponent({
  name: 'demo.vue',
  setup(_, context) {
      console.log()
    return {}
  },
  components: {},
})
</script>
<style lang='less' scoped>

</style>