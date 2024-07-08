
#Weather App

HTML CODE FILE:

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Weather App</title>
    <link rel="stylesheet" href="weather.css">
</head>

<body>
    <div class="nav-con">
        <div class="nav-bar">
            <img src="C:\Users\durga\OneDrive\Desktop\WeatherApp\images\cloud_29dp_5F6368_FILL0_wght400_GRAD0_opsz24.png"
                width="40px" height="50px">
            <div class="nav">
                <li>Home</li>
                <li>Map</li>
                <li>News</li>
                <li>Contact</li>
                <li><button>Get App</button></li>
            </div>
        </div>

        <div class="container">
            <div class="interface">
                <h1>Different Kind of Weather</h1>
                <h1>inside of 24/7 hrs</h1>
                <div class="news">
                    <p>You too often some very human culture artifacts really lead</p>
                    <p>Business down the certain routes</p>

                </div>
                <span class="material-icons">
                    Search
                </span>
                <input type="text" id="place" placeholder="Enter the City name">
                <button onclick="weather(document.queryselector('#place').value)">Get Update</button>
                <p>Best way to know your city weather</p>
            <div class="info">
                <div class="header">
                    <h1>Today Weather Report</h1>
                </div>
                <div class="report">
                    <img src="C:\Users\durga\OneDrive\Desktop\WeatherApp\images\weather_mix_48dp_5F6368_FILL0_wght400_GRAD0_opsz48.png" width="100px" height="100px">
                    <span id="description"></span>
                </div>
                <div class="output">
                    <div class="digit">
                        <h1 id="deg">0&deg;C</h1>
                        <span id="min">0&deg;C</span>
                        <span id="max">0&deg;C</span>

                    </div>
                    <div class="list-info">
                        <h3 id="wind">0mph</h3>
                        <h3 id="humidity">0%C</h3>

                    </div>
                    <div class="convertor">
                        <span id="celsius" onclick="con('celsius')">&deg;C</span>
                        <span id="fahrenheit" onclick="con('fahrenheit')">| &deg;F</span>

                    </div>
                </div>
            </div>
            </div>
            
            <script src="weather.js"></script>
</body>

</html>