# pak-e-commerce
creating a front end of the e-commerce site
<!DOCTYPE html>
<html>
<head>
  <title>Simple Calculator</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: Arial;
    }

    .calculator {
      border: 2px solid #333;
      padding: 20px;
      width: 220px;
    }

    #display {
      width: 100%;
      height: 40px;
      margin-bottom: 10px;
      text-align: right;
      font-size: 18px;
    }

    button {
      width: 45px;
      height: 40px;
      margin: 3px;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
</head>
<body>

<div class="calculator">
  <input type="text" id="display" disabled>

  <div>
    <button onclick="clearDisplay()">C</button>
    <button onclick="appendValue('/')">/</button>
    <button onclick="appendValue('*')">*</button>
    <button onclick="appendValue('-')">-</button>

    <button onclick="appendValue('7')">7</button>
    <button onclick="appendValue('8')">8</button>
    <button onclick="appendValue('9')">9</button>
    <button onclick="appendValue('+')">+</button>

    <button onclick="appendValue('4')">4</button>
    <button onclick="appendValue('5')">5</button>
    <button onclick="appendValue('6')">6</button>

    <button onclick="appendValue('1')">1</button>
    <button onclick="appendValue('2')">2</button>
    <button onclick="appendValue('3')">3</button>

    <button onclick="appendValue('0')">0</button>
    <button onclick="calculate()">=</button>
  </div>
</div>

<script>
  let display = document.getElementById("display");

  function appendValue(value) {
    display.value += value;
  }

  function clearDisplay() {
    display.value = "";
  }

  function calculate() {
    try {
      display.value = eval(display.value);
    } catch {
      display.value = "Error";
    }
  }
</script>

</body>
</html>

<img width="284" height="177" alt="images" src="https://github.com/user-attachments/assets/e137dd74-8413-47e5-8910-75950ce5689a" />
