<template>
    <div class="empty">
        <div>{{ title }}</div>
    </div>
</template>
<script>
  export default {
    name: 'EmptyValues',
    computed: {
      title () {
//        let vm = this
        console.log(this.$parent.emptyMsg)
        return this.$parent.emptyMsg
      }
    }
  }
</script>
<!--<style>-->
<!--.empty {-->
<!--}-->
<!--</style>-->