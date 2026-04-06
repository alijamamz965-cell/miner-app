<!DOCTYPE html>
<html>
<head>
    <script src="https://telegram.org"></script>
    <style>
        body { background: #000; color: #fff; text-align: center; font-family: sans-serif; }
        .coin { width: 200px; margin-top: 50px; cursor: pointer; border-radius: 50%; }
        .coin:active { transform: scale(0.95); }
    </style>
</head>
<body>
    <h1>انقر لتعدين عملتي</h1>
    <div id="score">0</div>
    <img src="رابط_صورة_عملتك" class="coin" onclick="tap()">
    <script>
        let count = 0;
        function tap() {
            count++;
            document.getElementById('score').innerText = count;
            window.Telegram.WebApp.HapticFeedback.impactOccurred('medium');
        }
    </script>
</body>
</html>
