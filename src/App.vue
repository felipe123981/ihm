<template>
  <div id="app">
    <div>
      <h3>Data:</h3>
      <center>
        <table border="1" id="clock_table">
          <tr>
            <td><input size="2" id="hours " type="text" placeholder="DD" /></td>
            <td>
              <input size="2" id="minutes" type="text" placeholder="MM" />
            </td>
            <td>
              <input size="4" id="seconds" type="text" placeholder="AAAA" />
            </td>
          </tr>
        </table>

        <h3>Horario:</h3>

        <table border="1" id="clock_table">
          <tr>
            <td><input size="2" id="hours" type="text" placeholder="HH" /></td>
            <td>
              <input size="2" id="minutes" type="text" placeholder="MM" />
            </td>
            <td>
              <input size="2" id="seconds" type="text" placeholder="SS" />
            </td>
          </tr>
        </table>
      </center>
    </div>
    <br />
    <div>
      <center>
        <h3>Temperatura:</h3>
        <table>
          <tr>
            <td>
              <h3>Tmp1</h3>

              <input type="text" size="3" :placeholder="temp" />
            </td>
            <td>
              <h3>Tmp2</h3>

              <input type="text" size="3" :placeholder="temp" />
            </td>
            <td>
              <h3>Tmp3</h3>

              <input type="text" size="3" :placeholder="temp" />
            </td>
            <td>
              <h3>pHsolo</h3>

              <input type="text" size="3" :placeholder="7.0" />
            </td>
          </tr>
        </table>
      </center>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      temp: "45 C°"
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#clock_table {
  border: black;
}
</style>
