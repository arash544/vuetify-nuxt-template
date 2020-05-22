<template>
  <div>
    <TopNavbar />
    <main>
      <section>
        <LogarithmicChart />
        <Calendar />
      </section>
      <section class="wrapper">
        <DoughnutChart />
        <section class="wrapper-statistics">
          <Bar />
          <Growth />
        </section>
        <div class="wrapper-text">
          <Txt />
          <Photos />
          <Icons />
        </div>
        <Buttons />
      </section>
    </main>
  </div>
</template>

<script>
import Calendar from "@/components/calendar-col/Calendar";
import Txt from "@/components/calendar-col/Txt";
import Photos from "@/components/calendar-col/Photos";
import Icons from "@/components/calendar-col/Icons";
import Buttons from "@/components/calendar-col/Buttons";
import DoughnutChart from "@/components/charts/DoughnutChart";
import LogarithmicChart from "@/components/charts/LogarithmicChart";
import Bar from "@/components/charts/Bar";
import Growth from "@/components/charts/Growth";
import TopNavbar from "@/components/navbar-part/TopNavbar";
export default {
  components: {
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
  }
};
</script>

<style lang="scss" scoped>
section {
  display: flex;
  flex-wrap: wrap;
}
.wrapper {
  display: flex;
  width: 100%;
}
main {
  padding-top: 120px;
  padding-left: 11%;
}
.wrapper-statistics {
  display: flex;
  flex-direction: column;
  margin-left: 20px;
  width: 30%;
}
.wrapper-text {
  display: flex;
  flex-direction: column;
  width: 28%;
}
</style>
