# Ex.08 Design of a Standard Calculator
## Date: 29/04/2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
calc.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colorful Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1 align="center">NITHISH KUMAR P(212221040115)</h1>
    <div class="calculator-container">
        <div class="calculator">
            <input type="text" id="display" readonly>
            <div class="buttons">
                <button onclick="appendToDisplay('(')">(</button>
                <button onclick="appendToDisplay(')')">)</button>
                <button onclick="appendToDisplay('^')">^</button>
                <button onclick="appendToDisplay('%')">%</button>
                <button onclick="appendToDisplay('1')">1</button>
                <button onclick="appendToDisplay('2')">2</button>
                <button onclick="appendToDisplay('3')">3</button>
                <button onclick="appendToDisplay('+')">+</button>
                <button onclick="appendToDisplay('4')">4</button>
                <button onclick="appendToDisplay('5')">5</button>
                <button onclick="appendToDisplay('6')">6</button>
                <button onclick="appendToDisplay('-')">-</button>
                <button onclick="appendToDisplay('7')">7</button>
                <button onclick="appendToDisplay('8')">8</button>
                <button onclick="appendToDisplay('9')">9</button>
                <button onclick="appendToDisplay('*')">*</button>
                <button onclick="clearDisplay()">C</button>
                <button onclick="appendToDisplay('0')">0</button>
                <button onclick="calculate()">=</button>
                <button onclick="appendToDisplay('/')">/</button>
            </div>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>


styles.css

.calculator-container {
    width: 300px;
    margin: 100px auto;
    background-color: #3498db; 
    padding: 20px; 
    border-radius: 10px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5); 
}

.calculator {
    text-align: center;
}

#display {
    width: 100%;
    height: 40px; 
    margin-bottom: 10px;
    padding: 10px;
    background-color: #1abc9c;
    color: white; 
    border: 2px solid #16a085; 
    border-radius: 5px; 
    font-size: 20px; 
    font-weight: bold; 
    text-align: right; 
    box-sizing: border-box; 
}

.buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr); 
    gap: 5px;
}

.buttons button {
    width: calc(100% - 10px); 
    height: 45px;
    margin: 0;
    padding: 0;
    font-size: 20px;
    background-color: #db3447; 
    color: white; 
    border: 2px solid #2980b9; 
    border-radius: 5px; 
    cursor: pointer;
    transition: background-color 0.3s ease; 
}

.buttons button:hover {
    background-color: #2980b9;
}

.buttons button:active {
    background-color: #1f8d65;
}

script.js

let display = document.getElementById('display');

function appendToDisplay(value) {
    display.value += value;
}

function clearDisplay() {
    display.value = '';
}

function calculate() {
    try {
        display.value = eval(display.value);
    } catch (error) {
        display.value = 'Error';
    }
}

```

## OUTPUT:

![alt text](<Screenshot (149).png>)
![alt text](<Screenshot (150).png>) 

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
