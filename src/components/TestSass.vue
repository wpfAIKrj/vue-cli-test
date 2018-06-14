<template>
  <div class="fullDiv">
    <p class="isPage">{{page}}</p>
    <p >{{showOne}}</p>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      page: '100',
      showOne: ''
    }
  },
  created: function () {
    let [one, two, three] = [1, 2, 3]
    this.showOne = one + two + three
    let eSet = new Set(['red', 'blue', 'green'])
    for (let item of eSet.keys()) {
      console.log(item)
    }

    for (let item of eSet.values()) {
      console.log(item)
    }

    eSet.forEach((value, key) => console.log(key + ':' + value))
    let numberSet = new Set([2, 4, 5])
    numberSet = new Set([...numberSet].map(x => x - 1))
    numberSet.forEach((value, key) => console.log('数字输出下：' + value))
    // 求交集并集
    let a = new Set([1, 2, 3, 4, 5])
    let b = new Set([3, 4, 12, 34, 2])
    let union = new Set([...a, ...b])
    console.log('输出下交集：' + union)
  },
  methods: {
    changeName: function (oldName = 'wang') {

    }
  }
}
</script>

<style lang="scss">
$pColor:#ff00ff;
.fullDiv {
  width: 100%;
  height: 100%;
  .isPage {
    margin-left: 100px;
    color: $pColor;
  }
}

</style>
