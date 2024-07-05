# JavaScript-Standard-Calculator


Design a Webpage using JavaScript of a Stanndard Calculator with a minimum of five mathematical operations.


## ALGORITHM

### Step 1: Setup the Project Structure

Create a folder for your project.
Inside this folder, create three files: index.html, style.css, and index.js.
Add the background image to your project directory (e.g., background-image.jpg).

### Step 2: HTML Structure

Open index.html and add the basic HTML structure.
Include links to the style.css and index.js files.

### Step 3: CSS Styling

Open style.css and add styles for the body, calculator, and buttons.

### Step 4: JavaScript Functionality

Open index.js and add functions for adding values to the display, clearing the display, and calculating the result.


## calculator.html

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">
    <script src="index.js" defer></script>
</head>
<body>
     <div class="name">
        <h1>&nbsp;&nbsp;&nbsp;&nbsp;Standard Calculator</h1>
        <h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Smriti M [212221040157]</h2>
     </div>    
     <div id="calculator">
        <input type="text" id="display">
        <br><br><br>
        <input type="button" value="7" onclick="addToDisplay('7')">
        <input type="button" value="8" onclick="addToDisplay('8')">
        <input type="button" value="9" onclick="addToDisplay('9')">
        <input type="button" value="/" onclick="addToDisplay('/')">
        <br>
        <input type="button" value="4" onclick="addToDisplay('4')">
        <input type="button" value="5" onclick="addToDisplay('5')">
        <input type="button" value="6" onclick="addToDisplay('6')">
        <input type="button" value="-" onclick="addToDisplay('-')">
        <br>
        <input type="button" value="1" onclick="addToDisplay('1')">
        <input type="button" value="2" onclick="addToDisplay('2')">
        <input type="button" value="3" onclick="addToDisplay('3')">
        <input type="button" value="+" onclick="addToDisplay('+')">
        <br>
        <input type="button" value="0" onclick="addToDisplay('0')">
        <input type="button" value="=" onclick="calculate()">
        <input type="button" value="*" onclick="addToDisplay('*')">
        <input type="button" value="%" onclick="addToDisplay('%')">
        <br>
        <input type="button" id="clear" value="C" onclick="clearDisplay()">
    </div>
</body>
</html>
```

## style.css

```
body {
    font-family: Arial, sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    margin: 0;
    background: url("bg.jpeg") no-repeat center center fixed;
    background-size: cover;
    flex-direction: column;
}

#calculator {
    border: 2px solid #b616a6;
    border-radius: 5px;
    padding: 60px;
    text-align: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    background-color: rgba(255, 255, 255, 0.8);
}

input[type="text"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    font-size: 18px;
}

input[type="button"] {
    width: 60px;
    height: 60px;
    font-size: 25px;
    margin: 5px;
    cursor: pointer;
    border-radius: 10px;
    font-weight: bolder;
    border: 4px solid rgb(13, 15, 14);
}

input[type="button"]:hover {
    background-color: #eee;
}

#clear {
    background-color: rgb(22, 231, 228);
    color: #fff;
}

#display {
    margin-right: 60px;
    border: 4px solid black;
}

.name {
    margin-bottom: 50px;
}

```

## index.js

```
function addToDisplay(value) {
    document.getElementById('display').value += value;
}

function clearDisplay() {
    document.getElementById('display').value = '';
}

function calculate() {
    try {
        document.getElementById('display').value = eval(document.getElementById('display').value);
    } catch (error) {
        document.getElementById('display').value = 'Error';
    }
}
```



## OUTPUT

<img width="959" alt="output" src="https://github.com/SmritiManikand/JavaScript-Standard-Calculator/assets/113674204/8e97065c-aae4-42b1-a1f9-71b8136359e3">

