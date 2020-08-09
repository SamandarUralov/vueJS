<template>
  <div class="App">
    <Date />
    <Chart />
    <Result />
  </div>
</template>

<script>
import Date from "./components/date";
import Chart from "./components/chart";
import Result from "./components/result";

export default {
  name: "App",
  components: {
    Date,
    Chart,
    Result,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen",
    "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue",
    sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.App {
  padding: 10px 150px 0 150px;
  background-color: #f5f6faff;
  height: 100vh;
}
@media (max-width: 768px) {
  .App {
    padding: 0;
  }
}
</style>
