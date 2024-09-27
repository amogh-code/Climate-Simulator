<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Climate Simulator</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f0f0f0;
            color: #333;
            margin: 0;
            padding: 0;
            transition: background-color 0.3s, color 0.3s;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .dark-mode {
            background-color: #2c2c2c;
            color: #e0e0e0;
        }
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 0;
            margin-bottom: 20px;
        }
        .slider-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
        }
        .dark-mode .slider-container {
            background-color: #3c3c3c;
            color: #e0e0e0;
        }
        .slider-label {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .graph-container {
            margin-top: 30px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            padding: 20px;
            transition: transform 0.3s ease;
        }
        .dark-mode .graph-container {
            background-color: #3c3c3c;
        }
        .graph-container:hover {
            transform: translateY(-5px);
        }
        canvas {
            width: 100%;
            height: 400px;
            border-radius: 5px;
        }
        button {
            padding: 12px 24px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.2s;
            font-size: 16px;
            font-weight: bold;
        }
        button:hover {
            background-color: #45a049;
            transform: translateY(-2px);
        }
        input[type="range"] {
            width: 60%;
            margin-left: 10px;
        }
        h1, h2, h3 {
            text-align: center;
            color: #333;
        }
        .dark-mode h1, .dark-mode h2, .dark-mode h3 {
            color: #e0e0e0;
        }
        .graph-description {
            margin-top: 10px;
            font-style: italic;
            text-align: center;
        }
        .info-section {
            margin-top: 50px;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .dark-mode .info-section {
            background-color: #3c3c3c;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div id="dateTime"></div>
            <button id="toggleButton" onclick="toggleDarkMode()">Toggle Dark Mode</button>
        </header>

        <h3 style="font-size: 12px;">|| Jai Guru Dev ||</h3>
        <h1>Anveshana 2025</h1>
        <h3>Done by Advaith, Hariprasad, and Amogh from Class 12 A SSRVM Bengaluru North</h3>
        <h2>Climate Simulator</h2>

        <form id="inputForm">
            <div class="slider-container">
                <label class="slider-label">Ocean Heat Absorption Coefficient (A_OCEAN): 
                    <input type="range" min="0" max="1" value="0.2" step="0.01" id="A_OCEAN" oninput="updateValue('A_OCEAN')">
                    <span id="A_OCEAN_value">0.20</span>
                </label>
                <label class="slider-label">Land Heat Absorption Coefficient (A_LAND): 
                    <input type="range" min="0" max="1" value="0.3" step="0.01" id="A_LAND" oninput="updateValue('A_LAND')">
                    <span id="A_LAND_value">0.30</span>
                </label>
                <label class="slider-label">Sea Ice Heat Absorption Coefficient (A_ICE): 
                    <input type="range" min="0" max="1" value="0.1" step="0.01" id="A_ICE" oninput="updateValue('A_ICE')">
                    <span id="A_ICE_value">0.10</span>
                </label>
                <label class="slider-label">Ice Melt Rate: 
                    <input type="range" min="0" max="0.1" value="0.05" step="0.001" id="ICE_MELT_RATE" oninput="updateValue('ICE_MELT_RATE')">
                    <span id="ICE_MELT_RATE_value">0.050</span>
                </label>
                <label class="slider-label">Time Steps (Years): 
                    <input type="range" min="10" max="200" value="100" id="TIME_STEPS" oninput="updateValue('TIME_STEPS')">
                    <span id="TIME_STEPS_value">100</span>
                </label>
                <label class="slider-label">Wind Magnitude (m/s): 
                    <input type="range" min="0" max="20" value="5" step="0.1" id="wind_magnitude" oninput="updateValue('wind_magnitude')">
                    <span id="wind_magnitude_value">5.0</span>
                </label>
                <label class="slider-label">Greenhouse Gases (normalized): 
                    <input type="range" min="0.5" max="2" value="1" step="0.01" id="greenhouse_gases" oninput="updateValue('greenhouse_gases')">
                    <span id="greenhouse_gases_value">1.00</span>
                </label>
            </div>
            <button type="submit">Generate Graphs</button>
        </form>

        <div class="graph-container">
            <canvas id="atmosphereTemp"></canvas>
            <p class="graph-description" id="atmosphereDesc">Atmospheric temperature over time based on user inputs.</p>
        </div>
        <div class="graph-container">
            <canvas id="oceanTemp"></canvas>
            <p class="graph-description" id="oceanDesc">Ocean temperature changes influenced by heat absorption coefficients.</p>
        </div>
        <div class="graph-container">
            <canvas id="landTemp"></canvas>
            <p class="graph-description" id="landDesc">Land temperature variations based on environmental factors.</p>
        </div>
        <div class="graph-container">
            <canvas id="iceVolume"></canvas>
            <p class="graph-description" id="iceDesc">Sea ice volume changes over time due to melting rates.</p>
        </div>

        <div class="info-section">
            <h3>About Climate Change and This Tool</h3>
            <p>Climate change is a long-term shift in global weather patterns and average temperatures. This simulator helps visualize the complex interactions between different components of the Earth's climate system.</p>
            <p>How to use this tool:</p>
            <ul>
                <li>Adjust the sliders to change various climate parameters.</li>
                <li>Click "Generate Graphs" to see how these changes affect the climate over time.</li>
                <li>Observe how different factors interact and influence each other.</li>
            </ul>
            <p>Key Facts:</p>
            <ul>
                <li>The Earth's average temperature has increased by about 1°C since pre-industrial times.</li>
                <li>Sea levels are rising at a rate of about 3.3 mm per year.</li>
                <li>Arctic sea ice is declining at a rate of 13% per decade.</li>
                <li>Human activities, particularly the burning of fossil fuels, are the primary driver of current climate change.</li>
            </ul>
        </div>
    </div>

    <script>
        function updateDateTime() {
            const now = new Date();
            document.getElementById('dateTime').innerText = now.toLocaleString();
        }

        function updateValue(sliderId) {
            const sliderValue = document.getElementById(sliderId).value;
            document.getElementById(sliderId + '_value').innerText = parseFloat(sliderValue).toFixed(3);
        }

        function toggleDarkMode() {
            document.body.classList.toggle('dark-mode');
            const button = document.getElementById('toggleButton');
            button.innerText = document.body.classList.contains('dark-mode') ? 'Toggle Light Mode' : 'Toggle Dark Mode';
            generateGraphs(new Event('submit'));
        }

        function generateGraphs(event) {
            event.preventDefault();

            const A_OCEAN = parseFloat(document.getElementById('A_OCEAN').value);
            const A_LAND = parseFloat(document.getElementById('A_LAND').value);
            const A_ICE = parseFloat(document.getElementById('A_ICE').value);
            const ICE_MELT_RATE = parseFloat(document.getElementById('ICE_MELT_RATE').value);
            const TIME_STEPS = parseInt(document.getElementById('TIME_STEPS').value);
            const wind_magnitude = parseFloat(document.getElementById('wind_magnitude').value);
            const greenhouse_gases = parseFloat(document.getElementById('greenhouse_gases').value);

            let atmosphere_temps = [];
            let ocean_temps = [];
            let land_temps = [];
            let sea_ice_volumes = [];

            let atmosphere_temp = 15; // Initial atmospheric temperature
            let ocean_temp = 10; // Initial ocean temperature
            let land_temp = 12; // Initial land temperature
            let sea_ice_volume = 100; // Initial sea ice volume

            const C_ATMOSPHERE = 1; // Heat capacity of the atmosphere
            const C_OCEAN = 10; // Heat capacity of the ocean
            const C_LAND = 5; // Heat capacity of the land

            for (let i = 0; i < TIME_STEPS; i++) {
                // Heat transfer calculations
                let heat_atmosphere_to_ocean = A_OCEAN * (atmosphere_temp - ocean_temp) / C_OCEAN;
                let heat_land_to_ocean = A_LAND * (land_temp - ocean_temp) / C_OCEAN;
                let heat_ocean_to_land = A_LAND * (ocean_temp - land_temp) / C_LAND;

                // Temperature updates
                atmosphere_temp += -heat_atmosphere_to_ocean * C_ATMOSPHERE + greenhouse_gases * 0.1;
                ocean_temp += heat_atmosphere_to_ocean + heat_land_to_ocean - A_ICE * sea_ice_volume / 1000;
                land_temp += heat_ocean_to_land + wind_magnitude * 0.01;

                // Sea ice volume update
                sea_ice_volume = Math.max(0, sea_ice_volume - ICE_MELT_RATE * (ocean_temp - 0));

                atmosphere_temps.push(atmosphere_temp);
                ocean_temps.push(ocean_temp);
                land_temps.push(land_temp);
                sea_ice_volumes.push(sea_ice_volume);
            }

            drawGraph('atmosphereTemp', atmosphere_temps, 'Atmospheric Temperature (°C)', 'rgba(255, 99, 132, 0.8)', TIME_STEPS);
            drawGraph('oceanTemp', ocean_temps, 'Ocean Temperature (°C)', 'rgba(54, 162, 235, 0.8)', TIME_STEPS);
            drawGraph('landTemp', land_temps, 'Land Temperature (°C)', 'rgba(75, 192, 192, 0.8)', TIME_STEPS);
            drawGraph('iceVolume', sea_ice_volumes, 'Sea Ice Volume (Million km³)', 'rgba(153, 102, 255, 0.8)', TIME_STEPS);

            // Update graph descriptions
            document.getElementById('atmosphereDesc').innerText = "Atmospheric temperature over time based on user inputs.";
            document.getElementById('oceanDesc').innerText = "Ocean temperature changes influenced by heat absorption coefficients.";
            document.getElementById('landDesc').innerText = "Land temperature variations based on environmental factors.";
            document.getElementById('iceDesc').innerText = "Sea ice volume changes over time due to melting rates.";
        }

        function drawGraph(canvasId, data, label, color, timeSteps) {
            const canvas = document.getElementById(canvasId);
            const ctx = canvas.getContext('2d');
            
            // Set canvas size
            canvas.width = canvas.offsetWidth;
            canvas.height = canvas.offsetHeight;
            
            const width = canvas.width;
            const height = canvas.height;
            const padding = 60;

            ctx.clearRect(0, 0, width, height);
            
            const minValue = 0;
            const maxValue = Math.max(...data);
            const valueRange = maxValue - minValue;

            // Draw background
            ctx.fillStyle = document.body.classList.contains('dark-mode') ? '#333' : '#f8f8f8';
            ctx.fillRect(0, 0, width, height);

            // Draw axes
            ctx.beginPath();
            ctx.moveTo(padding, padding);
            ctx.lineTo(padding, height - padding);
            ctx.lineTo(width - padding, height - padding);
            ctx.strokeStyle = document.body.classList.contains('dark-mode') ? '#ddd' : '#666';
            ctx.lineWidth = 2;
            ctx.stroke();

            // Draw graph
            ctx.beginPath();
            ctx.strokeStyle = color;
            ctx.lineWidth = 3;

            const xStep = (width - 2 * padding) / (data.length - 1);
            const yScale = (height - 2 * padding) / valueRange;

            for (let i = 0; i < data.length; i++) {
                const x = padding + i * xStep;
                const y = height - padding - (data[i] - minValue) * yScale;
                if (i === 0) {
                    ctx.moveTo(x, y);
                } else {
                    ctx.lineTo(x, y);
                }
            }

            ctx.stroke();

            // Add labels
            ctx.fillStyle = document.body.classList.contains('dark-mode') ? '#fff' : '#333';
            ctx.font = 'bold 16px Arial';
            ctx.textAlign = 'center';
            ctx.fillText(label, width / 2, 30);
            ctx.font = '14px Arial';
            ctx.fillText('Time (Years)', width / 2, height - 10);
            
            ctx.save();
            ctx.rotate(-Math.PI / 2);
            ctx.textAlign = 'center';
            ctx.fillText('Value', -height / 2, 20);
            ctx.restore();

            // Add scale
            ctx.textAlign = 'right';
            ctx.fillText(maxValue.toFixed(2), padding - 5, padding);
            ctx.fillText(minValue.toFixed(2), padding - 5, height - padding);

            // Draw grid lines
            ctx.strokeStyle = document.body.classList.contains('dark-mode') ? 'rgba(255,255,255,0.1)' : 'rgba(0,0,0,0.1)';
            ctx.lineWidth = 1;
            for (let i = 1; i < 5; i++) {
                const y = padding + (height - 2 * padding) * i / 5;
                ctx.beginPath();
                ctx.moveTo(padding, y);
                ctx.lineTo(width - padding, y);
                ctx.stroke();
            }
            for (let i = 1; i < 5; i++) {
                const x = padding + (width - 2 * padding) * i / 5;
                ctx.beginPath();
                ctx.moveTo(x, padding);
                ctx.lineTo(x, height - padding);
                ctx.stroke();
            }

            // Add X and Y axis coordinates
            ctx.fillStyle = document.body.classList.contains('dark-mode') ? '#fff' : '#333';
            ctx.font = '12px Arial';
            ctx.textAlign = 'center';
            for (let i = 0; i <= 5; i++) {
                const x = padding + (width - 2 * padding) * i / 5;
                const y = height - padding + 15;
                ctx.fillText((i * timeSteps / 5).toFixed(0), x, y);
            }
            ctx.textAlign = 'right';
            for (let i = 0; i <= 5; i++) {
                const y = padding + (height - 2 * padding) * i / 5;
                const value = minValue + (valueRange * i / 5);
                ctx.fillText(value.toFixed(2), padding - 10, y + 3);
            }
        }

        document.getElementById('inputForm').addEventListener('submit', generateGraphs);
        setInterval(updateDateTime, 1000);

        // Generate graphs on page load
        generateGraphs(new Event('submit'));
    </script>
</body>
</html>
