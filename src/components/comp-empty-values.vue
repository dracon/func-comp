<template>
    <div class="empty">
        <h1>{{ title }}</h1>
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
<style lang="scss">
.empty {
    h1{
        font-size: 10vw;
    }
}
</style>