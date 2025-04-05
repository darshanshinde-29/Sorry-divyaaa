<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Divya Sorry</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(to top right, #ffe0ec, #ffffff);
            text-align: center;
            padding: 50px;
            margin: 0;
            overflow: hidden;
            animation: backgroundShift 10s infinite alternate;
        }
        h1 {
            color: #ff4081;
            font-size: 48px;
            margin-bottom: 20px;
            animation: slideIn 1s ease-out;
        }
        p {
            font-size: 24px;
            color: #555;
            animation: fadeIn 2s ease-in;
        }
        .heart {
            font-size: 64px;
            color: #ff4081;
            animation: pulse 1.5s infinite;
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
        @keyframes slideIn {
            from { transform: translateY(-50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes floatUp {
            0% { transform: translateY(100%); opacity: 0; }
            50% { opacity: 1; }
            100% { transform: translateY(-100%); opacity: 0; }
        }
        @keyframes backgroundShift {
            0% { background-position: left top; }
            100% { background-position: right bottom; }
        }
        .floating-hearts, .floating-flowers, .floating-sparkles {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            overflow: hidden;
            pointer-events: none;
        }
        .floating-hearts span, .floating-flowers span, .floating-sparkles span {
            position: absolute;
            display: block;
            animation: floatUp 6s linear infinite;
            font-size: 24px;
        }
        .floating-flowers span {
            color: #ffb6c1;
        }
        .floating-sparkles span {
            color: gold;
        }
        .butterfly {
            position: absolute;
            top: 80%;
            left: -100px;
            font-size: 32px;
            animation: flyAcross 12s linear infinite;
        }
        @keyframes flyAcross {
            0% { transform: translate(0, 0) rotate(0); }
            50% { transform: translate(100vw, -50vh) rotate(45deg); }
            100% { transform: translate(200vw, -100vh) rotate(90deg); }
        }
    </style>
</head>
<body>
    <h1>Divya, I'm Really Sorry</h1>
    <p>I didn’t mean to hurt you. Please forgive me.</p>
    <div class="heart">❤️</div>
    <div class="floating-hearts">
        <span style="left: 10%; animation-delay: 0s;">❤️</span>
        <span style="left: 30%; animation-delay: 1s;">❤️</span>
        <span style="left: 50%; animation-delay: 2s;">❤️</span>
        <span style="left: 70%; animation-delay: 3s;">❤️</span>
        <span style="left: 90%; animation-delay: 4s;">❤️</span>
    </div>
    <div class="floating-flowers">
        <span style="left: 15%; animation-delay: 0s;">🌸</span>
        <span style="left: 40%; animation-delay: 2s;">🌼</span>
        <span style="left: 65%; animation-delay: 4s;">🌺</span>
    </div>
    <div class="floating-sparkles">
        <span style="left: 25%; animation-delay: 1s;">✨</span>
        <span style="left: 55%; animation-delay: 3s;">✨</span>
        <span style="left: 85%; animation-delay: 5s;">✨</span>
    </div>
    <div class="butterfly">🦋</div><!-- Background Music -->
<audio autoplay loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>

</body>
</html>
