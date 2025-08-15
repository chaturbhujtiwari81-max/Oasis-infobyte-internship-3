# Oasis-infobyte-internship-3
\\html code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Temperature Converter</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="converter-container">
        <h1>Temperature Converter</h1>

        <div class="input-group">
            <label for="tempInput">Enter Temperature:</label>
            <input type="number" id="tempInput" placeholder="e.g., 32">
        </div>

        <div class="radio-group">
            <input type="radio" id="celsius" name="tempUnit" value="celsius" checked>
            <label for="celsius">Celsius</label>

            <input type="radio" id="fahrenheit" name="tempUnit" value="fahrenheit">
            <label for="fahrenheit">Fahrenheit</label>
        </div>

        <button id="convertBtn">Convert</button>

        <div class="result-area">
            <p>Converted Temperature:</p>
            <p id="resultDisplay" class="result"></p>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
\\css code
body {
    font-family: Arial, sans-serif;
    background-color: #e6f7ff;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.converter-container {
    background-color: #fff;
    padding: 2.5rem;
    border-radius: 12px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    width: 350px;
}

h1 {
    color: #007bff;
    margin-bottom: 1.5rem;
}

.input-group, .radio-group {
    margin-bottom: 1.5rem;
}

input[type="number"] {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #ccc;
    border-radius: 6px;
    box-sizing: border-box;
}

.radio-group label {
    margin-right: 1.5rem;
    font-weight: bold;
}

button {
    background-color: #007bff;
    color: white;
    border: none;
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    border-radius: 6px;
    cursor: pointer;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #0056b3;
}

.result-area {
    margin-top: 1.5rem;
    border-top: 1px solid #eee;
    padding-top: 1rem;
}

.result {
    font-size: 1.5rem;
    font-weight: bold;
    color: #28a745;
}
