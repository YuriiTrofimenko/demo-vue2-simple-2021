<template lang="pug">
.counter(@click="increase") {{count}}
</template>

<script>
export default {
  name: 'Counter',
  props: {
    initialCount: Number
  },
  data: function () {
    return {
      count: this.initialCount
    }
  },
  methods: {
    increase: function(){
      this.count++
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
.counter
  color darkred
  font-size 48px
  font-family 'Times New Roman', Times, serif
</style>