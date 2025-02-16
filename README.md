<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sliding Puzzle Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
        }
        #puzzle {
            width: 320px;
            height: 320px;
            margin: 50px auto;
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            grid-gap: 2px;
        }
        .tile {
            width: 78px;
            height: 78px;
            background-color: #333;
            color: white;
            font-size: 24px;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
        }
        .empty {
            background-color: #f4f4f4;
            cursor: default;
        }
    </style>
</head>
<body>
    <h1>Sliding Puzzle Game</h1>
    <div id="puzzle"></div>
    <button onclick="shuffle()">Shuffle</button>
    <script>
        const puzzle = document.getElementById('puzzle');
        const size = 4;
        let tiles = [];

        function createTiles() {
            tiles = [];
            for (let i = 0; i < size * size - 1; i++) {
                const tile = document.createElement('div');
                tile.classList.add('tile');
                tile.textContent = i + 1;
                tile.addEventListener('click', moveTile);
                tiles.push(tile);
            }
            tiles.push(document.createElement('div')); // empty tile
        }

        function renderTiles() {
            puzzle.innerHTML = '';
            tiles.forEach(tile => {
                tile.classList.contains('tile') ? tile.classList.remove('empty') : tile.classList.add('empty');
                puzzle.appendChild(tile);
            });
        }

        function shuffle() {
            for (let i = tiles.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [tiles[i], tiles[j]] = [tiles[j], tiles[i]];
            }
            renderTiles();
        }

        function moveTile() {
            const index = tiles.indexOf(this);
            const emptyIndex = tiles.indexOf(document.querySelector('.empty'));
            const validMoves = [emptyIndex - 1, emptyIndex + 1, emptyIndex - size, emptyIndex + size];

            if (validMoves.includes(index)) {
                [tiles[index], tiles[emptyIndex]] = [tiles[emptyIndex], tiles[index]];
                renderTiles();
            }
        }

        createTiles();
        renderTiles();
    </script>
</body>
</html>
