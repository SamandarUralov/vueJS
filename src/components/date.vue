<template>
  <div class="date_line">
    <h2 class="date_name">Поступления</h2>
    <div class="date_box">
      <span class="calendar">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          style="background-color: #ff8989ff"
          viewBox="0 0 24 24"
          fill="white"
          width="18px"
          height="18px"
        >
          <path d="M0 0h24v24H0z" fill="none" />
          <path
            d="M9 11H7v2h2v-2zm4 0h-2v2h2v-2zm4 0h-2v2h2v-2zm2-7h-1V2h-2v2H8V2H6v2H5c-1.11 0-1.99.9-1.99 2L3 20c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 16H5V9h14v11z"
          />
        </svg>
      </span>
      <span class="date">May 02.2020 - Iyun 02.2020</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Date",
};
</script>

<style>
.date_line {
  width: 100%;
  display: flex;
  justify-content: center;
  padding: 20px 40px 20px 20px;
  display: flex;
  justify-content: space-between;
}
.date_box {
  width: 25%;
  padding: 10px;
  display: flex;
  font-size: 13px;
  box-shadow: 0 0 5px #ddd;
  background-color: #fff;
  font-weight: bold;
  color: #999;
}
.calendar {
  margin-left: 5px;
  width: 20%;
  color: #ff8989ff;
}
.date {
  display: flex;
  justify-content: center;
  width: 80%;
}
@media (max-width: 768px) {
  .date_line {
    padding: 10px;
    flex-direction: column;
    align-items: center;
  }
  .date_box {
    width: 70%;
    border-radius: 2px;
  }
}
@media (max-width: 900px) {
  .date_line {
    text-align: center;
  }
  .date_name {
    margin-bottom: 15px;
  }
}
</style>
