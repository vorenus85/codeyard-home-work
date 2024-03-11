<script>
import LeftSide from './LeftSide.vue'
import RightSide from './RightSide.vue'

export default {
  components: { LeftSide, RightSide }
}
</script>
<template>
  <div class="p-2">
    <div id="layout" class="grid">
      <LeftSide />
      <RightSide />
    </div>
  </div>
</template>
