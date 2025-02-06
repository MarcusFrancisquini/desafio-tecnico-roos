<template>
  <div
    class="scroll-horizontal"
    ref="scrollContainer"
    @mousedown="startDrag"
    @mousemove="drag"
    @mouseup="stopDrag"
    @mouseleave="stopDrag"
    @touchstart="startDrag"
    @touchmove="drag"
    @touchend="stopDrag"
    @touchcancel="stopDrag"
  >
    <!-- conteúdo -->
    <slot></slot>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isDragging: false,
      startX: 0,
      scrollLeft: 0,
    }
  },
  methods: {
    startDrag(e) {
      this.isDragging = true
      // posição inicial do mouse
      const pageX = e.pageX || e.touches[0].pageX
      this.startX = pageX
      // posição inicial do scroll
      this.scrollLeft = this.$refs.scrollContainer.scrollLeft
      // alteração do cursor
      this.$refs.scrollContainer.style.cursor = 'grabbing'
    },
    drag(e) {
      if (!this.isDragging) return
      e.preventDefault()
      // nova posição do mouse
      const pageX = e.pageX || e.touches[0].pageX
      // calcula a diferença de posições
      const distance = pageX - this.startX
      // move o conteúdo
      this.$refs.scrollContainer.scrollLeft = this.scrollLeft - distance
    },
    stopDrag() {
      this.isDragging = false
      // alteração do cursor
      this.$refs.scrollContainer.style.cursor = 'grab'
    },
  },
}
</script>
