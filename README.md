<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Click the Button Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            text-align: center;
        }

        #game-container {
            width: 100%;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
        }

        #click-btn {
            padding: 20px 40px;
            font-size: 20px;
            background-color: #3498db;
            color: white;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            position: absolute;
        }

        #score-board {
            position: fixed;
            top: 10px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 24px;
            background-color: #2c3e50;
            color: white;
            padding: 10px 20px;
            border-radius: 10px;
        }

        #timer {
            font-size: 18px;
            color: red;
        }
    </style>
</head>
<body>
    <div id="score-board">Score: <span id="score">0</span> | Time Left: <span id="timer">30</span>s</div>
    <div id="game-container">
        <button id="click-btn">Click Me!</button>
    </div>

    <script>
        let score = 0;
        let timeLeft = 30;
        let timer;

        // Function to start the game
        function startGame() {
            document.getElementById('click-btn').style.display = 'block';
            score = 0;
            timeLeft = 30;
            document.getElementById('score').textContent = score;
            document.getElementById('timer').textContent = timeLeft;

            timer = setInterval(() => {
                timeLeft--;
                document.getElementById('timer').textContent = timeLeft;
                if (timeLeft <= 0) {
                    clearInterval(timer);
                    alert('Game Over! Final Score: ' + score);
                    document.getElementById('click-btn').style.display = 'none';
                }
            }, 1000);
        }

        // Function to move the button randomly
        function moveButton() {
            const btn = document.getElementById('click-btn');
            const maxWidth = window.innerWidth - btn.offsetWidth;
            const maxHeight = window.innerHeight - btn.offsetHeight;

            const randomX = Math.floor(Math.random() * maxWidth);
            const randomY = Math.floor(Math.random() * maxHeight);

            btn.style.left = randomX + 'px';
            btn.style.top = randomY + 'px';
        }

        // Event listener for button click
        document.getElementById('click-btn').addEventListener('click', function() {
            score++;
            document.getElementById('score').textContent = score;
            moveButton();
        });

        // Start the game when the page loads
        window.onload = startGame;
    </script>
</body>
</html>
