<template>
  <div>
    <img src="../assets/demo/filter_bg.jpg" style="width: 100%">
    <search @result-click="resultClick" @change="getResult" :results="results" :value.sync="value"></search>
  </div>
</template>

<script>
import Search from '../components/Search'
export default {
  components: {
    Search
  },
  methods: {
    resultClick: function (item) {
      alert('you click the result item: ' + JSON.stringify(item))
    },
    getResult: function (val) {
      this.results = getResult(this.value)
    }
  },
  data () {
    return {
      results: [],
      value: ''
    }
  }
}

function getResult (val) {
  let rs = []
  for (let i = 0; i < 9; i++) {
    rs.push({
      title: `${val} result: ${i + 1} `,
      other: i
    })
  }
  return rs
}
</script>