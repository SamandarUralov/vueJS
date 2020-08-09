<template>
  <div class="left_result">
    <div class="first_left_result">
      <div class="first_box_left_result">
        <p class="name_box">Начисления</p>
        <h3>+6.000.000</h3>
      </div>
      <div class="first_left_result_right">
        <div class="first_box_right_result">
          <h3>вы работали:</h3>
          <div class="day_result">
            <h2>20</h2>
            <p>дня</p>
          </div>
          <div class="hour_result">
            <h2>160</h2>
            <p>часов</p>
          </div>
        </div>
        <div class="info_right_box">
          Рабочих дней в Июне месяце -
          <span>22</span>
          дня; Виходных -
          <span>9</span>
        </div>
      </div>
    </div>

    <div class="result_bottom_info">
      <h5>Оклад по штатному расписанию</h5>
      <p>+ 2.000.000</p>
    </div>
    <div class="result_bottom_info">
      <h5>Оклад по штатному расписанию</h5>
      <p>+ 350.000</p>
    </div>
    <div class="result_bottom_info">
      <h5>Оклад по штатному расписанию</h5>
      <p>+ 200.000</p>
    </div>
    <div class="result_bottom_info">
      <h5>Оклад по штатному расписанию</h5>
      <p>+ 800</p>
    </div>
    <div class="result_bottom_info">
      <h5>Оклад по штатному расписанию</h5>
      <p>+ 2.000.000</p>
    </div>
    <div class="result_bottom_info">
      <h5>Оклад по штатному расписанию</h5>
      <p>+ 150.000</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "LeftSide",
};
</script>
<style>
.left_result {
  /* height: 420px; */
  border-radius: 5px;
  padding: 30px;
  width: 100%;
  background-color: white;
}
.first_box_left_result {
  width: 50%;
}
.first_left_result_right {
  width: 50%;
}
.first_left_result {
  display: flex;
  justify-content: space-between;
  padding-bottom: 20px;
  border-bottom: 1px solid #ccc;
}
.first_box_right_result {
  display: flex;
  justify-content: space-between;
}
.first_box_right_result > h3 {
  color: #333;
}
.day_result {
  color: orange;
}
.hour_result {
  color: #777;
}
.info_right_box {
  color: #888;
  font-weight: 600;
  font-size: 14px;
  margin-top: 10px;
  display: flex;
}
.info_right_box > span {
  color: black;
}
.result_bottom_info {
  display: flex;
  justify-content: space-between;
  padding: 10px;
  border-bottom: 1px solid #ccc;
}
.result_bottom_info > h5 {
  color: #333;
  font-size: 14px;
}
.result_bottom_info > p {
  color: #00c86fff;
  font-weight: bold;
}
@media (max-width: 768px) {
  /* .left_result {
    margin: 100px;
  } */
  .first_left_result {
    width: 100%;
    display: flex;
    flex-direction: column;
  }
  .first_box_right_result {
    justify-content: space-between;
  }
  .first_box_left_result {
    width: 100%;
    display: flex;
    justify-content: space-between;
  }
  .first_box_left_result > p {
    font-size: 18px;
    color: #333;
  }
  .first_left_result_right {
    width: 100%;
    margin: 15px 0;
  }
  .first_box_right_result > h3 {
    font-size: 16px;
  }
  .result_bottom_info > p {
    font-size: 14px;
    width: 30%;
  }
  .result_bottom_info > h5 {
    width: 70%;
    font-size: 14px;
  }
}
</style>