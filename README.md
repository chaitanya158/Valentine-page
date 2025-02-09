<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #ffcccb;
            font-family: Arial, sans-serif;
            flex-direction: column;
        }
        h1 {
            color: #d32f2f;
            font-size: 2.5em;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 1.2em;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: 0.3s;
        }
        .yes {
            background-color: #4CAF50;
            color: white;
        }
        .yes:hover {
            background-color: #388E3C;
        }
        .no {
            background-color: #d32f2f;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

    <h1>Will You Be My Valentine? ❤️</h1>
    <div class="buttons">
        <button class="yes" onclick="alert('Yay! ❤️')">Yes</button>
        <button class="no" id="noButton">No</button>
    </div>

    <script>
        document.getElementById("noButton").addEventListener("mouseover", function() {
            let x = Math.random() * window.innerWidth - 100;
            let y = Math.random() * window.innerHeight - 50;
            this.style.left = `${x}px`;
            this.style.top = `${y}px`;
        });
    </script>

</body>
</html>
