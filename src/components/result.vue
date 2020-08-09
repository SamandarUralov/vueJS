<template>
  <div class="result">
    <!-- <div class="result_into"> -->
    <LeftSide class="left" />
    <RightSide class="right" />
    <!-- </div> -->
  </div>
</template>
<script>
import LeftSide from "./left_side";
import RightSide from "./right_side";

export default {
  name: "Result",
  components: {
    LeftSide,
    RightSide,
  },
};
</script>
<style>
.result {
  height: 410px;
  width: 100%;
  margin: 20px 0;
  display: flex;
  flex-direction: row;
  padding: 20px 50px 20px 20px;
  justify-content: space-between;
}
/* .result_into {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
} */
.left {
  width: 65%;
}
.right {
  width: 35%;
}
@media (max-width: 768px) {
  .result {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .left {
    width: 100%;
  }
  .right {
    width: 100%;
  }
  /* .result_into {
    display: flex;
    flex-direction: column;
    width: 73%;
  } */
}
@media (max-width: 900px) {
  .result {
    height: 0;
    margin: 0;
    padding: 20px;
  }
}
</style>