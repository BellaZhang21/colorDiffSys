<template>
  <div>
    <ve-histogram :data="chartData" :colors="color"></ve-histogram>
  </div>
</template>

<script>
import Vue from 'vue'
import VCharts from 'v-charts'
Vue.use(VCharts)

export default {
  data () {
    return {
      chartData: {
        columns: ['日期', '销售量', '销售额'],
        rows: [
          { '日期': '1月1日', '销售量': 123, '销售额': 120 },
          { '日期': '1月2日', '销售量': 1223, '销售额': 780 },
          { '日期': '1月3日', '销售量': 2123, '销售额': 200 },
          { '日期': '1月4日', '销售量': 4123, '销售额': 300 },
          { '日期': '1月5日', '销售量': 3123, '销售额': 600 },
          { '日期': '1月6日', '销售量': 7123, '销售额': 800 }
        ]
      },
      color: ['#aaa', '#abc']
    }
  }
}
</script>
