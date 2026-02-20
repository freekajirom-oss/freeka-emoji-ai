# freeka-emoji-ai
Freeka Emoji AI - Text to Emoji Generator
<input type="text" id="textInput" placeholder="Type: pain success money">
<button onclick="generateEmoji()">Generate</button>
<div id="result"></div>

<script>
    const emojiDict = {
        pain: "💔",
        success: "🚀",
        money: "💰",
        music: "🎤",
        dream: "🌙"
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
