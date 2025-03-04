<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🎂 Birthday Countdown for Lakshmi Priya 🎉</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background: url('https://www.transparenttextures.com/patterns/hearts.png') red;
            color: #fff;
            overflow: hidden;
        }
        h1 {
            font-size: 36px;
            margin-top: 20px;
            animation: fadeIn 2s ease-in-out;
        }
        #countdown {
            font-size: 30px;
            font-weight: bold;
            color: #ffe600;
            margin-top: 20px;
            animation: bounce 1.5s infinite;
        }
        #birthdayMessage {
            display: none;
            font-size: 28px;
            color: #ff5733;
            font-weight: bold;
            margin-top: 30px;
            animation: zoomIn 2s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        @keyframes zoomIn {
            0% { transform: scale(0); }
            100% { transform: scale(1); }
        }
        @keyframes fireworks {
            0% { transform: scale(0); opacity: 1; }
            100% { transform: scale(1.5); opacity: 0; }
        }
        .firework {
            position: absolute;
            width: 15px;
            height: 15px;
            background-color: yellow;
            border-radius: 50%;
            animation: fireworks 1.5s ease-out infinite;
        }
    </style>
</head>
<body>
    <h1>🎂 Birthday Countdown for Lakshmi Priya 🎉</h1>
    <p>Time left until her next birthday:</p>
    <p id="countdown"></p>
    <p id="birthdayMessage">🎉 Happy Birthday, Lakshmi Priya! 🥳🎂🎁</p>
    <audio id="birthdaySong" src="https://www.fesliyanstudios.com/play-mp3/387" preload="auto"></audio>
    
    <script>
        function updateCountdown() {
            const birthday = new Date("December 15, 2025 00:00:00");
            const now = new Date();
            const timeDiff = birthday - now;
            
            const days = Math.floor(timeDiff / (1000 * 60 * 60 * 24));
            const hours = Math.floor((timeDiff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((timeDiff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((timeDiff % (1000 * 60)) / 1000);
            
            if (timeDiff > 0) {
                document.getElementById("countdown").innerText = `${days} days, ${hours} hours, ${minutes} minutes, ${seconds} seconds left!`;
            } else {
                document.getElementById("countdown").style.display = "none";
                document.getElementById("birthdayMessage").style.display = "block";
                playBirthdayMusic();
                startFireworks();
            }
        }
        
        function playBirthdayMusic() {
            let song = document.getElementById("birthdaySong");
            song.play();
        }
        
        function startFireworks() {
            for (let i = 0; i < 50; i++) {
                let firework = document.createElement("div");
                firework.classList.add("firework");
                firework.style.left = Math.random() * window.innerWidth + "px";
                firework.style.top = Math.random() * window.innerHeight + "px";
                firework.style.animationDuration = (Math.random() * 1 + 1) + "s";
                document.body.appendChild(firework);
                setTimeout(() => { firework.remove(); }, 1500);
            }
        }

        updateCountdown();
        setInterval(updateCountdown, 1000);
    </script>
</body>
</html>
