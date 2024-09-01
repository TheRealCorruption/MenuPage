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
            background-color: Light Red;
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
        .timeline-x {
            display: none;
        }
        .timeline-x h2 {
            background: linear-gradient(to right, rainbow, white);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .timeline-x .small-buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 5px;
        }
        .timeline-x .small-buttons button {
            font-size: 12px;
            padding: 5px;
        }
        .timeline-x .large-buttons {
            margin-top: 20px;
        }
        .timeline-x .large-buttons button {
            padding: 10px;
            width: 150px;
        }
        /* New gradient colors */
        #logs-section h2 {
            background: linear-gradient(to right, Bright green);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        #timeline-section h2 {
            background: linear-gradient(to right, lightblue, white);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        #discoverys-section h2 {
            background: linear-gradient(to right, purple, pink);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        #doi-section h2 {
            background: linear-gradient(to right, red, white);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Audio tag for background music -->
        <audio id="bg-music" autoplay loop>
            <source src="https://www.youtube.com/embed/TAyErJUq8Io?autoplay=1&loop=1&playlist=TAyErJUq8Io&mute=0" type="audio/mp3">
            Your browser does not support the audio element.
        </audio>

        <div class="section" id="logs-section">
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
        <div class="section" id="timeline-section">
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
        <div class="section" id="discoverys-section">
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
        <div class="section" id="doi-section">
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

        <!-- Timeline X section -->
        <div class="timeline-x" id="timeline-x-section">
            <h2>Timeline X</h2>
            <hr>
            <div class="small-buttons">
                <!-- Small floating buttons -->
                <button>File-#1</button>
                <button>File-#2</button>
                <button>File-#3</button>
                <button>File-#4</button>
                <button>File-#5</button>
                <button>File-#6</button>
                <button>File-#7</button>
                <button>File-#8</button>
                <button>File-#9</button>
                <button>File-#10</button>
                <button>File-#11</button>
                <button>File-#12</button>
                <button>File-#13</button>
                <button>File-#14</button>
                <button>File-#15</button>
                <button>File-#16</button>
                <button>File-#17</button>
                <button>File-#18</button>
                <button>File-#19</button>
                <button>File-#20</button>
            </div>
            <hr>
            <div class="large-buttons">
                <!-- Larger buttons -->
                <button>Cameras</button>
                <button>Entries</button>
                <button>Boss-TData</button>
                <button>Soul,Data</button>
            </div>
            <hr>
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
            video.muted = false; // Unmute the music after autoplay starts
            document.getElementById('boss-section').style.display = 'block';
        }

        // Function to randomly activate Timeline X
        function activateTimelineX() {
            const bossSection = document.getElementById('boss-section');
            const timelineXSection = document.getElementById('timeline-x-section');
            if (Math.random() > 0.5) {
                timelineXSection.style.display = 'block';
                bossSection.style.display = 'none';
                // Disable the BOSS section when Timeline X is active
            } else {
                timelineXSection.style.display = 'none';
                bossSection.style.display = 'block';
            }
        }

        document.addEventListener('DOMContentLoaded', function () {
            // Show new section and music after a 25-minute delay (1500000 milliseconds)
            setTimeout(activateNewSection, 1500000);

            // Check for activating Timeline X randomly every 15 minutes (900000 milliseconds)
            setInterval(activateTimelineX, 900000);
        });
    </script>
</body>
</html>
