<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Glitchy Interface</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
        }
        .container {
            padding: 20px;
        }
        h2 {
            color: white;
        }
        .button-row {
            margin-bottom: 20px;
        }
        button {
            background-color: black;
            color: white;
            border: 2px solid white;
            padding: 10px;
            margin: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: gray;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hidden YouTube video for background music -->
        <iframe id="bg-music" width="0" height="0" src="https://www.youtube.com/embed/TAyErJUq8Io?autoplay=1&loop=1&playlist=TAyErJUq8Io&mute=1" frameborder="0" allow="autoplay"></iframe>

        <div class="section">
            <h2>LOGS</h2>
            <div class="button-row">
                <button onclick="openLink('https://scratch.mit.edu/projects/1061726554/', this)">Tape-#1</button>
                <button onclick="openLink('', this)">Tape-#2</button>
                <button onclick="openLink('', this)">Tape-#3</button>
                <button onclick="openLink('', this)">Tape-#4</button>
                <button onclick="openLink('', this)">Tape-#5</button>
                <button onclick="openLink('', this)">Tape-#6</button>
                <button onclick="openLink('', this)">Tape-#7</button>
                <button onclick="openLink('', this)">Tape-#8</button>
            </div>
        </div>
        <div class="section">
            <h2>TIMELINE-FILES</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">T-#1</button>
                <button onclick="openLink('', this)">T-#2</button>
                <button onclick="openLink('', this)">T-#3</button>
                <button onclick="openLink('', this)">T-#4</button>
                <button onclick="openLink('', this)">T-#5</button>
                <button onclick="openLink('', this)">T-#6</button>
                <button onclick="openLink('', this)">T-#7</button>
                <button onclick="openLink('', this)">T-#8</button>
            </div>
        </div>
        <div class="section">
            <h2>DISCOVERYS</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">D-#1</button>
                <button onclick="openLink('', this)">D-#2</button>
                <button onclick="openLink('', this)">D-#3</button>
                <button onclick="openLink('', this)">D-#4</button>
                <button onclick="openLink('', this)">D-#5</button>
                <button onclick="openLink('', this)">D-#6</button>
                <button onclick="openLink('', this)">D-#7</button>
                <button onclick="openLink('', this)">D-#8</button>
            </div>
        </div>
        <div class="section">
            <h2>DATA-ON-INHABITENTS</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">DOI-#1</button>
                <button onclick="openLink('', this)">DOI-#2</button>
                <button onclick="openLink('', this)">DOI-#3</button>
                <button onclick="openLink('', this)">DOI-#4</button>
                <button onclick="openLink('', this)">DOI-#5</button>
                <button onclick="openLink('', this)">DOI-#6</button>
                <button onclick="openLink('', this)">DOI-#7</button>
                <button onclick="openLink('', this)">DOI-#8</button>
            </div>
        </div>
    </div>

    <script>
        function openLink(url, button) {
            if (url) {
                window.open(url, '_blank');
            } else {
                button.textContent = 'DATANOTFOUND'.split('')
                    .map(char => Math.random() > 0.5 ? char.toUpperCase() : char.toLowerCase())
                    .join('');
            }
        }

        // Unmute the video after a delay to bypass browser restrictions
        window.addEventListener('load', function() {
            const video = document.getElementById('bg-music');
            setTimeout(() => {
                const src = video.src.replace('&mute=1', '&mute=0');
                video.src = src;
            }, 1000); // 1-second delay to unmute
        });
    </script>
</body>
</html>
