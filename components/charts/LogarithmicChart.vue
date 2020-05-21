<template>
  <highcharts class="chart" :options="chartOptions"></highcharts>
</template>

<script>
export default {
  name: "LogarithmicChart",
  data() {
    return {
      chartOptions: {
        title: {
          text: "Time Spendings!"
        },
        series: [
          {
            data: [100, 22, 165, 44, 423, 333]
          }
        ]
      },
      resultdata: 0
    };
  },
  created() {
    // fetch('https://jsonplaceholder.ir/todos')
    // .then(res=>res.json())
    // .then(rs=>{
    //   this.resultdata = rs
    // })
    let count = 0;

    setInterval(() => {
      // this.resultdata = count++
    }, 1000);
  },
  watch: {
    resultdata(newValue) {
      this.chartOptions.series[0].data.push(newValue);
    }
  }
};
</script>

<style lang="scss" scoped>
.chart {
  width: 65%;
  height: 300px;
  border: 1px solid rgb(219, 215, 215);
  box-shadow:$shadow;
  position: absolute;
  top: 330px;
  left: 44%;
  transform: translate(-50%, -50%);
  text-align: center;
  @media only screen and (max-width: 768px) {
    margin-top: 300px;
    margin-left: 32.5px;
    width: 100%;
    position: absolute;
  }
}
</style>