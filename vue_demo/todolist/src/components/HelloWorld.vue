<template>
  <li class="item" @click="deletesss">{{content}}</li>
</template>

<script>
export default {
  props: ['content', 'index'],
  methods: {
    deletesss: function () {
      this.$emit('delete', this.index)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
  .item {
    color: green;
  }
</style>
