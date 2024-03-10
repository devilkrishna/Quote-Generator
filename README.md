# Quote-Generator
By using these code you can create an amazing quote. By using your good name
<!DOCTYPE html>
<html>
<head>
    <title>Random Quote Generator</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background-image: url('path/to/your/background/image.jpg');
            background-size: cover;
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-position: center;
        }
    </style>
</head>
<body>
    <div class="container mt-5">
        <h1 class="text-center mb-4">Random Quote Generator</h1>
        <div class="input-group mb-3">
            <input type="text" id="nameInput" class="form-control" placeholder="Enter your name">
            <button class="btn btn-primary" onclick="generateQuote()">Generate Quote</button>
        </div>
        <div id="quoteOutput" class="mt-3"></div>
    </div>

    <script>
        function generateQuote() {
            const name = document.getElementById('nameInput').value;
            const quotes = [
                `"${name}, the only way to do great work is to love what you do."`,
                `"${name}, life is 10% what happens to us and 90% how we react to it."`,
                `"${name}, success is not the key to happiness. Happiness is the key to success."`,
                `"${name}, the only limit to our realization of tomorrow will be our doubts of today."`,
                `"${name}, 𝙉𝙤𝙩𝙝𝙞𝙣𝙜 𝙩𝙚𝙖𝙘𝙝𝙚𝙨 𝙪𝙨 𝙗𝙚𝙩𝙩𝙚𝙧 𝙩𝙝𝙖𝙣 𝙤𝙪𝙧 𝙤𝙬𝙣 𝙚𝙭𝙥𝙚𝙧𝙞𝙚𝙣𝙘𝙚𝙨."`
                `"${name}, The danger with friends is that once they stop talking to you, they will start talking about you.."`
                `"${name}, THE HARDEST BATTLE IS BETWEEN WHAT U KNOW IN YOUR HEAD & WHAT U FEEL IN YOUR HEART."`
                `"${name}, believe you can and you're halfway there."`
            ];
            const randomQuote = quotes[Math.floor(Math.random() * quotes.length)];
            document.getElementById('quoteOutput').innerHTML = `<p class="lead">${randomQuote}</p>`;
        }
    </script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.min.js"></script>
</body>
</html>

