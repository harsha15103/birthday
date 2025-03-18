<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Madamji!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            text-align: center;
            color: white;
            margin: 0;
            padding: 0;
        }
        .container {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }
        p {
            font-size: 1.5rem;
            max-width: 600px;
        }
        .cake {
            font-size: 5rem;
            margin: 20px 0;
        }
        .btn {
            background: white;
            color: #ff6699;
            padding: 10px 20px;
            font-size: 1.2rem;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }
        .btn:hover {
            background: #ff6699;
            color: white;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Happy Birthday, Madamji! 🎉</h1>
        <p>Dear Rashi,</p>
        <p>Wishing you a day filled with love, joy, and all the happiness in the world. You are special, and you deserve the best!</p>
        <div class="cake">🎂</div>
        <button class="btn" onclick="alert('Have an amazing birthday, Madamji! 🎈🎊')">Click for a Surprise!</button>
        
        <!-- Background Music -->
        <audio id="birthdaySong" autoplay>
            <source src="your-audio-file.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        
        <script>
            const audio = document.getElementById("birthdaySong");
            audio.currentTime = 31; // Start at 31 seconds
            
            audio.addEventListener("timeupdate", function() {
                if (audio.currentTime >= 60) { // Stop at 1 minute
                    audio.pause();
                }
            });
        </script>
    </div>
</body>
</html>

