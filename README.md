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
        .new-section {
            display: none;
            margin-top: 20px;
        }
        .new-section h2 {
            color: red;
            background: linear-gradient(to right, red, silver, gold);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .new-section button {
            background: linear-gradient(to right, purple, pink);
            color: white;
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

        <!-- New section to appear after a delay -->
        <div class="new-section" id="boss-section">
            <h2>BOSS's Of The Abyss</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">Null</button>
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

        // Function to play new music and show the new section
        function activateNewSection() {
            const video = document.getElementById('bg-music');
            video.src = 'https://www.youtube.com/embed/u3pQzhQPEis?autoplay=1&loop=1&playlist=u3pQzhQPEis&mute=0';

            const newSection = document.getElementById('boss-section');
            newSection.style.display = 'block';
        }

        // Trigger the new section and music change after a random delay between 30 minutes and 2 hours
        window.addEventListener('load', function() {
            const delay = Math.floor(Math.random() * (120 - 30 + 1) + 30) * 60000; // Random delay between 30 and 120 minutes
            setTimeout(activateNewSection, delay);
        });

        // Unmute the original video after a delay to bypass browser restrictions
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
