<!DOCTYPE html>
<html>
<head>
<style>
   body{
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      background-color: rgb(203, 243, 243);
   }
   input,span{
      font-size: 20px;
   }
</style>
</head>
<body>
<h1>Temperature Converter</h1>
<h2>Type Temperature in celcius to convert it into fahrenheit</h2>
<p>
<label>Celcius :</label>
<input id="celcius" type="number" placeholder="Celcius"
oninput="converter(this.value)" onchange="converter(this.value)">
</p>
<p>Fahrenheit: <span class="fahrenheit"></span></p>
<script>
   function converter(temp) {
      document.querySelector(".fahrenheit").innerHTML=(temp-32)/1.8;
   }
</script>
</body>
</html>
