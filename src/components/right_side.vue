<template>
  <div class="right_result">
    <div class="right_result_top">
      <p>Курс валют</p>
      <div class="kurs_info">
        <div class="kurs_info_box">
          <p style="color: #999; width: 15% ">USD</p>
          <p class="kurs_num">
            <span>
              <IconIncrease />
            </span>
            <span>10210.00</span>
          </p>
          <p class="kurs_num">
            <span>
              <IconDecrease />
            </span>
            <span>10251.00</span>
          </p>
        </div>
        <div class="kurs_info_box">
          <p style="color: #999; width: 15% ">EURO</p>
          <p class="kurs_num">
            <span>
              <IconIncrease />
            </span>
            <span>11000.00</span>
          </p>
          <p class="kurs_num">
            <span>
              <IconDecrease />
            </span>
            <span>11700.00</span>
          </p>
        </div>
      </div>
    </div>
    <div class="right_result_bottom">
      <div class="right_bottom">
        <div class="right_bottom_num">679.330</div>
        <div class="right_bottom_text">Базовая расчетная величина (сум)</div>
      </div>
      <div class="right_bottom">
        <div class="right_bottom_num">223.000</div>
        <div class="right_bottom_text">минимальный размер заработной платы (сум)</div>
      </div>
      <div class="right_bottom">
        <div class="right_bottom_num">12.5%</div>
        <div class="right_bottom_text">Подоходный налог %</div>
      </div>
      <p>Обновлено: 01.02.2020</p>
    </div>
  </div>
</template>
<script>
import IconDecrease from "./iconDecrease";
import IconIncrease from "./iconIncrease";
export default {
  name: "RightSide",
  components: {
    IconDecrease,
    IconIncrease,
  },
};
</script>
<style >
.right_result {
  margin-left: 20px;
  width: 100%;
  /* height: 420px; */
}
.right_result_top {
  height: 30%;
  border-radius: 5px;
  padding: 10px 35px;
  margin-bottom: 20px;
  background-color: white;
}
.right_result_bottom {
  height: 65%;
  border-radius: 5px;
  background-color: white;
  display: flex;
  flex-direction: column;
  padding: 15px 15px 0 15px;
}
.right_result_top > p {
  color: #333;
  font-weight: bold;
  margin-bottom: 10px;
}
.kurs_info_box {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.kurs_info_box > p {
  font-weight: bold;
  font-size: 14px;
  color: #666;
}
.kurs_num {
  display: flex;
  margin-bottom: 10px;
}
.kurs_num > span {
  margin: 0 5px;
}

.right_bottom {
  display: flex;
  flex-direction: row;
  margin-bottom: 25px;
  height: 70%;
}
.right_bottom_num {
  width: 40%;
  padding: 10px 0;
  font-weight: bold;
  font-size: 18px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #e9f6fcff;
}
.right_bottom_text {
  display: flex;
  font-size: 15px;
  justify-content: center;
  align-items: center;
  margin-left: 15px;
  font-weight: bold;
  color: #777;
  width: 60%;
}
.right_result_bottom > p {
  color: #777;
  font-size: 12px;
  margin-bottom: 10px;
}
@media (max-width: 768px) {
  .right_result {
    margin-left: 0;
  }
}
</style>