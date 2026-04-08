<!DOCTYPE html>
<html>
<head>
    <title>BAI Mining</title>
    <style>
        body { text-align: center; background: #000; color: #fff; font-family: Arial; }
        .coin { width: 200px; cursor: pointer; transition: transform 0.1s; margin-top: 50px; }
        .coin:active { transform: scale(0.9); }
        #balance { font-size: 2em; margin-top: 20px; color: #ffd700; }
    </style>
</head>
<body>
    <h1>BAI Coin Mining ⛏️</h1>
    <div id="balance">0</div>
    <img src="https://placeholder.com" class="coin" onclick="mine()">
    <script>
        let score = 0;
        function mine() {
            score += 10;
            document.getElementById('balance').innerText = score;
        }
    </script>
</body>
</html>
