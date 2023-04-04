<!DOCTYPE html>
<html>
<head>
	<title>Scientific Calculator</title>
	<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
	<script src="calculator.js"></script>
	<style>
		#calculator {
			margin: 50px auto;
			width: 300px;
			height: auto;
			border: 1px solid #000;
			padding: 10px;
			text-align: center;
		}
		#graph {
			margin: 50px auto;
			width: 600px;
			height: 400px;
			border: 1px solid #000;
			padding: 10px;
		}
		input {
			font-size: 20px;
			padding: 10px;
			margin: 5px;
			width: 80%;
			border: none;
			border-bottom: 1px solid #000;
			text-align: right;
		}
		button {
			font-size: 20px;
			padding: 10px;
			margin: 5px;
			width: 40%;
			border: none;
			background-color: #ccc;
			cursor: pointer;
		}
		button:hover {
			background-color: #ddd;
		}
	</style>
</head>
<body>
	<div id="calculator">
		<input type="text" id="input">
		<br>
		<button onclick="insert('sin(')">sin</button>
		<button onclick="insert('cos(')">cos</button>
		<button onclick="insert('tan(')">tan</button>
		<button onclick="insert('^')">^</button>
		<br>
		<button onclick="insert('sqrt(')">√</button>
		<button onclick="insert('log(')">log</button>
		<button onclick="insert('ln(')">ln</button>
		<button onclick="insert('(')">(</button>
		<br>
		<button onclick="insert('7')">7</button>
		<button onclick="insert('8')">8</button>
		<button onclick="insert('9')">9</button>
		<button onclick="insert(')')">)</button>
		<br>
		<button onclick="insert('4')">4</button>
		<button onclick="insert('5')">5</button>
		<button onclick="insert('6')">6</button>
		<button onclick="insert('+')">+</button>
		<br>
		<button onclick="insert('1')">1</button>
		<button onclick="insert('2')">2</button>
		<button onclick="insert('3')">3</button>
		<button onclick="insert('-')">-</button>
		<br>
		<button onclick="insert('0')">0</button>
		<button onclick="insert('.')">.</button>
		<button onclick="calculate()">=</button>
		<button onclick="insert('*')">*</button>
		<br>
		<button onclick="clearInput()">Clear</button>
	</div>
	<div id="graph">
	</div>
</body>
</html>
