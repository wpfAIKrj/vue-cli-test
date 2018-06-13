<template>
  <p class="isPage">{{page}}</p>
</template>

<script>
export default {
  data: function() {
    return {
      page:'100'
    }
  },
  methods: {
    changeName: function(oldName='wang') {

    }
  }
}
</script>

<style lang="scss">
$pColor:#ff00ff;
.isPage {
  margin-left: 100px;
  color: $pColor;
}
</style>
