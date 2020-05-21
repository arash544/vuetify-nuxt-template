<template>
<div>
  <TopNavbar/>
  <LogarithmicChart/>
  <Calendar/>
  <DoughnutChart/>
  <Bar/>
  <Growth/>
  <Txt/>
  <Photos/>
  <Icons/>
  <Buttons/>
</div>

</template>

<script>
import Calendar from '@/components/calendar-col/Calendar'
import Txt from '@/components/calendar-col/Txt'
import Photos from '@/components/calendar-col/Photos'
import Icons from '@/components/calendar-col/Icons'
import Buttons from '@/components/calendar-col/Buttons'
import DoughnutChart from '@/components/charts/DoughnutChart'
import LogarithmicChart from '@/components/charts/LogarithmicChart'
import Bar from '@/components/charts/Bar'
import Growth from '@/components/charts/Growth'
import TopNavbar from '@/components/navbar-part/TopNavbar'
export default {
  components:{
    Calendar,
    TopNavbar,
    DoughnutChart,
    LogarithmicChart,
    Bar,
    Growth,
    Txt,
    Photos,
    Icons,
    Buttons
  },

}
</script>

<style scoped>

</style>
