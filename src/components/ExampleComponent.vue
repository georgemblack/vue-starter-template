<template>
  <div class="example-component">
    <button @click="testAction">
      Button
    </button>
    <p>Value: {{ testValue }}</p>
  </div>
</template>

<script>
import { mapActions, mapGetters} from 'vuex'

export default {
  name: 'ExampleComponent',
  computed: {
    ...mapGetters(['testValue'])
  },
  methods: {
    ...mapActions(['testAction'])
  }
}
</script>

<style lang="scss" scoped>
</style>
