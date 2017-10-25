<template>
    <div id="app">
        <func-comp :items="myItems"></func-comp>
    </div>
</template>

<script>
    import FuncComp from './components/func-comp.vue'
    import EmptyValues from './components/comp-empty-values.vue'
    import ListValues from './components/comp-list-values.vue'

    export default {
    name: 'app',
    components: {
      FuncComp, EmptyValues, ListValues
    },
    data () {
      return {
        msg: 'Welcome to Your Vue.js App',
        myItems: [
          {
            name: 'Wolfgang'
          },
          {
            name: 'Elisabeth'
          },
          {
            name: 'Linda'
          }
        ]
      }
    }
  }
</script>

<style lang="scss">
body {
    background-color: aquamarine;

}
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }

    h1, h2 {
        font-weight: normal;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
