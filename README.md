<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Valentine</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
            background: pink;
            text-align: center;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
        }
        #no {
            position: absolute;
        }
    </style>
</head>
<body>
    <div>
        <h1>Will you be my Valentine, Tabassum? ❤️</h1>
        <button onclick="alert('Yay! ❤️')">Yes</button>
        <button id="no" onmouseover="move()">No</button>
    </div>

    <script>
        function move() {
            const x = Math.random() * window.innerWidth;
            const y = Math.random() * window.innerHeight;
            document.getElementById("no").style.left = x + "px";
            document.getElementById("no").style.top = y + "px";
        }
    </script>
</body>
</html>
