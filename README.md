<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Crush Button</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Do you have a crush?</h1>
        <button id="crushButton">Crush</button>
        <p id="message" class="hidden">You have a crush!</p>
    </div>

    <script src="script.js"></script>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
}

.container {
    text-align: center;
    background-color: white;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1 {
    color: #333;
}

button {
    background-color: #ff4081;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #e91e63;
}

.hidden {
    display: none;
}

#message {
    margin-top: 20px;
    font-size: 18px;
    color: #4caf50;
}
document.getElementById('crushButton').addEventListener('click', function() {
    document.getElementById('message').classList.toggle('hidden');
});
