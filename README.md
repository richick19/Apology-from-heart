<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Apology Letter</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe6e6;
        }
        .container {
            display: none;
            margin-top: 50px;
            padding: 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
        }
        .heart {
            color: red;
            font-size: 30px;
            position: absolute;
            animation: burst 1.5s linear infinite;
        }
        @keyframes burst {
            0% { transform: scale(0); opacity: 1; }
            100% { transform: scale(3); opacity: 0; }
        }
    </style>
</head>
<body>
    <button onclick="showMessage()">Start</button>
    <div id="messageContainer" class="container">
        <p><strong>Dear Shreta,</strong></p>
        <p>I sincerely apologize for the actions of my past self. I deeply regret any inconvenience or difficulty I have caused you.</p>
        <p>It was never my intention to bully or hurt your feelings, and I take full responsibility for my actions. I am genuinely sorry for that. Please feel free to let me know if there is anything I can do to make amends.</p>
        <p><strong>Yours sincerely,</strong><br>Richick</p>
    </div>
    <script>
        function showMessage() {
            document.getElementById('messageContainer').style.display = 'inline-block';
            burstHearts();
        }
        function burstHearts() {
            for (let i = 0; i < 20; i++) {
                let heart = document.createElement('div');
                heart.innerHTML = "❤️";
                heart.classList.add('heart');
                document.body.appendChild(heart);
                heart.style.left = Math.random() * window.innerWidth + 'px';
                heart.style.top = Math.random() * window.innerHeight + 'px';
                setTimeout(() => heart.remove(), 1500);
            }
        }
    </script>
</body>
</html># Apology-from-heart
