<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>🔥 Freeka Emoji AI 🔥</title>
    <link rel="icon" type="image/png" href="logo.png">
    <style>
        body {
            background-color: #111; /* sombre */
            color: #ff0066; /* texte Freeka */
            text-align: center;
            font-family: 'Arial Black', sans-serif;
            padding: 50px;
        }
        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        h3 {
            font-weight: normal;
            margin-bottom: 40px;
        }
        input[type=text] {
            padding: 10px;
            width: 60%;
            font-size: 1em;
            border-radius: 8px;
            border: none;
            margin-bottom: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 1em;
            font-weight: bold;
            border-radius: 8px;
            border: none;
            background-color: #ff0066;
            color: white;
            cursor: pointer;
        }
        #result {
            margin-top: 30px;
            font-size: 2em;
        }
    </style>
</head>
<body>
    <h1>🔥 Freeka Emoji AI 🔥</h1>
    <h3>Transforme tes mots en emojis 🎤💔🚀</h3>

    <input type="text" id="textInput" placeholder="Tape ici: pain success money">
    <br>
    <button onclick="generateEmoji()">Généré</button>

    <div id="result"></div>

    <script>
        const emojiDict = {
            pain: "💔",
            success: "🚀",
            money: "💰",
            music: "🎤",
            dream: "🌙",
            fire: "🔥",
            star: "⭐",
            love: "❤️",
            sad: "😢",
            happy: "😎",
            party: "🥳",
            sleep: "😴",
            angel: "👼",
            devil: "😈",
            crown: "👑",
            guitar: "🎸",
            piano: "🎹",
            lightning: "⚡",
            moon: "🌕",
            sun: "☀️",
            ghost: "👻",
            diamond: "💎",
            wave: "🌊",
            coffee: "☕",
            skull: "💀",
            trophy: "🏆",
            robot: "🤖",
            cat: "🐱",
            dog: "🐶"
        };

        function generateEmoji() {
            let text = document.getElementById("textInput").value.toLowerCase();
            let words = text.split(" ");
            let result = "";

            words.forEach(word => {
                if (emojiDict[word]) {
                    result += emojiDict[word];
                }
            });

            document.getElementById("result").innerHTML = result;
        }
    </script>
</body>
</html>
