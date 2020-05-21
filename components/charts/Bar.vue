<template>
  <highcharts class="chart" :options="plotOptions"></highcharts>
</template>

<script>
export default {
  name: "Bar",
  data() {
    return {
      plotOptions: {
        chart: {
          type: "bar"
        },
        title: {
          text: "Level",
          text: "Congratulaition, you are at 71."
        },
        xAxis: {
          categories: ["Apples"]
        },
        yAxis: {
          min: 0,
          title: {
            text: "Total fruit"
          }
        },
        legend: {
          reversed: true
        },

        series: [
          {
            name: "John",
            data: [71]
          }
        ]
      }
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
  width: 30%;
  height: 170px;
  border: 1px solid rgb(219, 215, 215);
  box-shadow: $shadow;
  position: absolute;
  top: 640px;
  left: 61.5%;
  transform: translate(-50%, -50%);
  text-align: center;
  @media only screen and (max-width: 768px) {
    margin-top: 600px;
    margin-left: -61.32px;
    width: 100%;
    position: absolute;
    
  }
}
</style>