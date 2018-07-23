<template>
  <div class="singer">
    singer
  </div>
</template>

<script>
import { getSingerList } from 'api/singer'
export default {
  created() {
    this._getSingerList()
  },
  methods: {
    _getSingerList() {
      getSingerList().then((res) => {
        console.log(res.data)
      })
    }
  }
}
</script>

<style lang="stylus" scoped>
</style>
