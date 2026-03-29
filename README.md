<!DOCTYPE html>
<html>
<head>
    <title>Priyu Calculator</title>
    <style>
        body {
            text-align: center;
            font-family: Arial;
        }
        input {
            width: 200px;
            height: 30px;
            font-size: 18px;
            margin: 10px;
        }
        button {
            width: 50px;
            height: 40px;
            font-size: 18px;
            margin: 5px;
        }
    </style>
</head>
<body>

<h2>My Calculator 🔥</h2>

<input type="text" id="result" disabled><br>

<button onclick="addToDisplay('1')">1</button>
<button onclick="addToDisplay('2')">2</button>
<button onclick="addToDisplay('3')">3</button>
<button onclick="addToDisplay('+')">+</button><br>

<button onclick="addToDisplay('4')">4</button>
<button onclick="addToDisplay('5')">5</button>
<button onclick="addToDisplay('6')">6</button>
<button onclick="addToDisplay('-')">-</button><br>

<button onclick="addToDisplay('7')">7</button>
<button onclick="addToDisplay('8')">8</button>
<button onclick="addToDisplay('9')">9</button>
<button onclick="addToDisplay('*')">*</button><br>

<button onclick="clearDisplay()">C</button>
<button onclick="addToDisplay('0')">0</button>
<button onclick="calculate()">=</button>
<button onclick="addToDisplay('/')">/</button>

<script>
function addToDisplay(value) {
    document.getElementById("result").value += value;
}

function clearDisplay() {
    document.getElementById("result").value = "";
}

function calculate() {
    let exp = document.getElementById("result").value;
    document.getElementById("result").value = eval(exp);
}
</script>

</body>
</html>
