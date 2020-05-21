<template>
   <highcharts class="chart" :options="chartOptions"></highcharts>
</template>

<script>
export default {
    name:'LogarithmicChart',
  data() {
    return {
      
      chartOptions: {
            title: {
            text: 'Statistics'
    },
   
        series: [{
        type: 'pie',
        name: 'Browser share',
          data: [['Chrome', 58.9],
            ['Firefox', 13.29],
            ['Internet Explorer', 13],
            ['Edge', 3.78],
            ['Safari', 3.42],
            {
                name: 'Other',
                y: 7.61,
                dataLabels: {
                    enabled: false
                }
            }] ,
          
        }]
      },
      resultdata:0,
    
    }
    
  },
    created(){
    // fetch('https://jsonplaceholder.ir/todos')
    // .then(res=>res.json())
    // .then(rs=>{
    //   this.resultdata = rs
    // })
    let count=0
    
    setInterval(() => {
        // this.resultdata = count++
    }, 1000);
  },
  watch: {
    resultdata(newValue){

       this.chartOptions.series[0].data.push(newValue)
    }
  },
}
</script>

<style lang="scss" scoped>
.chart{
  width:32%;
  height: 350px;
  border:1px solid rgb(219, 215, 215);
  box-shadow: $shadow;
  position: absolute;
  top: 730px;
  left: 27.5%;
  transform: translate(-50%, -50%);
  text-align: center;
      @media only screen and (max-width: 768px) {
    margin-top: 240px;
    margin-left: 120.5px;
    width: 100%;
    position:absolute;
  
}
}
</style>