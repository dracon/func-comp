<script>
    import EmptyValues from './comp-empty-values.vue'
    import ListValues from './comp-list-values.vue'

  export default {
    functional: true,
    name: 'FuncComp',
    render: function (createElement, context) {
      function appropriateListComponent () {
        let items = context.props.items

        if (items.length === 0) {
          return EmptyValues
        } else {
          return ListValues
        }
      }
      return createElement(
        appropriateListComponent(),
        context.data,
        context.children
      )
    },
    props: {
      items: {
        type: Array,
        required: true
      }
    }
  }
</script>