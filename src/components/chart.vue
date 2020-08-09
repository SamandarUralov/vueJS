<template>
  <div class="chart md-layout md-gutter md-alignment-center">
    <div class="chart_box md-layout-item md-medium-size-33 md-small-size-35 md-xsmall-size-100">
      <div class="chart_box_left">
        <div class="chart_box_into">
          <p class="name_box">Начисления</p>
          <h3>6.000.000</h3>
          <p class="persentage">
            <span class="persentage_icon">
              <IconIncrease />
            </span>
            <span class="persentage_num">0.22%</span>
          </p>
        </div>
        <div class="line_chart">
          <ReactChart blue="blue" />
        </div>
      </div>
      <!-- <div class="chart_box_right"></div> -->
    </div>
    <div class="chart_box md-layout-item md-medium-size-33 md-small-size-35 md-xsmall-size-100">
      <div class="chart_box_left">
        <div class="chart_box_into">
          <p class="name_box">Удержано</p>
          <h3>5.000.000</h3>
          <p class="persentage">
            <span class="persentage_icon">
              <IconIncrease />
            </span>
            <span class="persentage_num">5.16%</span>
          </p>
        </div>
        <div class="line_chart">
          <ReactChart red="red" />
        </div>
      </div>
      <!-- <div class="chart_box_right"></div> -->
    </div>
    <div class="chart_box md-layout-item md-medium-size-33 md-small-size-35 md-xsmall-size-100">
      <div class="chart_box_left">
        <div class="chart_box_into">
          <p class="name_box">С начала года</p>
          <h3>14.000.000</h3>
          <p class="persentage">
            <span class="persentage_icon">
              <IconDecrease />
            </span>
            <span class="persentage_num decrease_num">0.74%</span>
          </p>
        </div>
        <div class="line_chart">
          <ReactChart orange="orange" />
        </div>
      </div>
      <!-- <div class="chart_box_right"></div> -->
    </div>
    <div
      id="chart_box_id"
      class="chart_box md-layout-item md-medium-size-33 md-small-size-35 md-xsmall-size-100"
    >
      <div class="chart_box_left">
        <div class="chart_box_into">
          <p class="name_box oklad">Должостной оклад</p>
          <h3>5.000.000</h3>
        </div>
        <div class="line_chart">
          <ReactChart green="green" />
        </div>
        <!-- <div class="chart_box_right"></div> -->
      </div>
    </div>
  </div>
</template>

<script>
import ReactChart from "./react_charts";
import IconIncrease from "./iconIncrease";
import IconDecrease from "./iconDecrease";

export default {
  name: "Chart",
  components: {
    ReactChart,
    IconIncrease,
    IconDecrease,
  },
};
</script>

<style>
.chart {
  flex: 4;
  display: flex;
  padding: 20px 40px;
  flex-wrap: wrap;
  flex-direction: row;
  justify-content: space-between;
}
.chart_box {
  flex: 1;
  height: 110px;
  padding: 15px 20px;
  margin-right: 25px;
  background-color: #fff;
  border-radius: 5px;
  border: 2px solid white;
}
.chart_box_left {
  display: flex;
  flex-direction: row;
}
.chart_box:hover {
  border: 2px solid #0054ffff;
  cursor: pointer;
  border-radius: 5px;
}
.chart_box_into > h3 {
  margin-bottom: 5px;
  color: #333;
}
.name_box {
  color: #333;
  font-size: 14px;
  margin-bottom: 5px;
  font-weight: bold;
}
.persentage {
  display: flex;
  font-size: 13px;
  font-weight: bold;
}
.persentage_num {
  margin-left: 8px;
  color: #00c86fff;
}
.decrease_num {
  color: #ff8989ff;
}
.day_result {
  display: flex;
}
.hour_result {
  display: flex;
}
.day_result > p {
  margin-right: 5px;
}
.hour_result > p {
  margin-right: 5px;
}
.chart_box_into {
  width: 50%;
}
.line_chart {
  width: 45%;
}
@media (max-width: 768px) {
  .chart {
    flex: 4;
    padding: 20px;
    justify-content: space-between;
  }
  .oklad {
    font-size: 12px;
    color: #999;
  }
  .chart_box {
    flex: 2;
    margin: 5px;
    width: 20.6%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>
