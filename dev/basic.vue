<template lang="jade">
.container
  a(href="https://github.com/vue-comps/vue-position-after-transform/blob/master/dev/basic.vue") source
  p width: 100px; height: 50px
  pat(style="width: 100px;height: 50px")
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px
  pat(style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, valign="center"
  pat(valign="center" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, valign="bottom"
  pat(valign="bottom" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, halign="right"
  pat(halign="right" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, halign="center"
  pat(halign="center" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px
  pat(style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, halign="right"
  pat(halign="right" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, halign="center"
  pat(halign="center" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
    patc.rotate Test
  p width: 100px; height: 50px; padding: 10px, halign="justify"
  pat(halign="justify" style="width: 100px;height: 50px; padding: 10px")
    patc.rotate Test
    patc.rotate Test
</template>

<script lang="coffee">
module.exports =
  components:
    "pat": require "../pat.js"
    "patc": require "../patc.js"
</script>

<style lang="stylus">
.vc-pat
  border 1px solid black
.vc-patc
  border 1px dashed black
.vc-pat-container
  border 1px dotted black
.rotate
  transform rotate(-45deg)
  //transform-origin top left
.container > a
  position absolute
  line-height 350px
  text-align center
  left 0
  bottom 0
  top 0
  right 0

</style>
