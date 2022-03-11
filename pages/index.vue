<template>
  <div class="w-full h-full flex items-center justify-center re">
    <h1 class="text-3xl font-bold underline">{{ $t('test') }}</h1>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
}
</script>
<style lang="scss" scoped>
.re {
  color: blue;
  position: absolute;
  top: 0px;
  bottom: 0px;
  left: 0px;
  right: 0px;
}
</style>
