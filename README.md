# Webapp

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Web App</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        input {
            padding: 10px;
            font-size: 16px;
            margin-top: 10px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin-top: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <h1>Welcome to the Simple Web App</h1>
    <p>Enter your name and click the button to get a greeting!</p>
    
    <input type="text" id="nameInput" placeholder="Enter your name">
    <button onclick="greetUser()">Greet Me!</button>
    
    <p id="greetingMessage"></p>

    <script>
        function greetUser() {
            const name = document.getElementById('nameInput').value;
            const greetingMessage = document.getElementById('greetingMessage');
            
            if (name) {
                greetingMessage.textContent = `Hello, ${name}! Welcome to our simple web app.`;
            } else {
                greetingMessage.textContent = 'Please enter your name!';
            }
        }
    </script>
    
</body>
</html>
