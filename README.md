<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Glitchy Interface</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <div class="section">
            <h2>LOGS</h2>
            <div class="button-row">
                <button onclick="openLink('https://scratch.mit.edu/projects/1061726554/', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
            </div>
        </div>
        <div class="section">
            <h2>TIMELINE-FILES</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
            </div>
        </div>
        <div class="section">
            <h2>DISCOVERYS</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
            </div>
        </div>
        <div class="section">
            <h2>DATA-ON-INHABITENTS</h2>
            <div class="button-row">
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
                <button onclick="openLink('', this)">BUTTON</button>
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
    </script>
</body>
</html>
