<template>
    <div class="list">
        <h2>{{ title }}</h2>
        <div class="list-item" v-for="item in $parent.myItems">{{ item.name }}</div>
    </div>
</template>
<script>
  export default {
    name: 'ListValues',
    data () {
      return {
        title: 'Vi er hjemme'
      }
    }
  }
</script>
<style lang="scss">
    .list {
        background: #0b143c;
        color: white;
        .list-item {
            color: #ffc400;
            padding: 1em 2em;
        }
    }
</style>