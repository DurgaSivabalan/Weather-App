
# Project Title

A brief description of what this project does and who it's for


#Weather App

JAVASCRIPT CODE FILE:

//variables
var temp,
    maxtemp,
    mintemp,
    desc,
    wind,
    hum,
    main,
    day,
    night;

//weather
var x = ["clear sky",
    "few clouds",
    "scatter clouds",
    "tornado",
    "shower rain",
    "mist", "thunderstorms", "rain", "snow", "haze", "broken clouds", "drizzle"];

//source
var y = ["C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img1.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img2.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img3.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img4.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img5.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img6.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img7.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img8.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img9.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img10.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img11.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img12.png",]

var z = ["C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img1.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img2.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img3.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img4.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img5.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img6.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img7.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img8.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img9.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img10.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img11.png",
    "C:\Users\durga\OneDrive\Desktop\WeatherApp\images\img12.png",]
function weather(input) {
    var city=input;
    alert(city);
}
var im = document.querySelector('#icon');
var myurl = "https://api.openweathermap.org/data/2.5/weather?";
var key = "171f49b1e118272e6e3adffca767b994";
var url=myurl+"appid="+key+"&units=metric&q"+city;
    alert(url);
    //fetch()
    .then(function (response) {
        console.log(response);
        return response.json();
    })
    .then(function (data) {
        console.log(data);
        temp = data.main.temp;
        document.querySelector("#deg").innerHTML = Math.round(temp) + "&deg;C"
        mintemp = data.main.temp - min;
        document.querySelector("#min").innerHTML = Math.round(mintemp) + "&deg;C"
        maxtemp = data.main.temp - max;
        document.querySelector("#max").innerHTML = "/" + Math.round(maxtemp) + "&deg;C"
        wind = data.wind.speed;
        document.querySelector("#wind").innerHTML = Math.round(wind) + "mph";
        hum = data.main.humidity;
        document.querySelector("#hum").innerHTML = hum + "%";
        desc = data.weather[0].description;
        document.querySelector("#description").innerHTML = desc;
    })
//condition
var dn = data.dt;
//alert(dn);
day = data.sys.sunrise;
night = data.sys.sunset;
if (dn >= night) {
    switch (desc) {
        case x[0]:
            im.src = z[0];
            break;
        case x[1]:
            im.src = z[1];
            break;
        case x[2]:
            im.src = z[2];
            break;
        case x[3]:
            im.src = z[3];
            break;
        case x[4]:
            im.src = z[4];
            break;
        case x[5]:
            im.src = z[5];
            break;
        case x[6]:
            im.src = z[6];
            break;
        case x[7]:
            im.src = z[7];
            break;
        case x[8]:
            im.src = z[8];
            break;
        case x[9]:
            im.src = z[9];
            break;
        case x[10]:
            im.src = z[10];
            break;
        case x[11]:
            im.src = z[11];
            break;
        case x[12]:
            im.src = z[12];
            break;
    }
}
else (dn >= day)
switch (desc) {
    case x[0]:
        im.src = y[0];
        break;
    case x[1]:
        im.src = y[1];
        break;
    case x[2]:
        im.src = y[2];
        break;
    case x[3]:
        im.src = yz[3];
        break;
    case x[4]:
        im.src = y[4];
        break;
    case x[5]:
        im.src = y[5];
        break;
    case x[6]:
        im.src = y[6];
        break;
    case x[7]:
        im.src = y[7];
        break;
    case x[8]:
        im.src = y[8];
        break;
    case x[9]:
        im.src = y[9];
        break;
    case x[10]:
        im.src = y[10];
        break;
    case x[11]:
        im.src = y[11];
        break;
    case x[12]:
        im.src = y[12];
        break;
}
//function end
function con(detector) {
    if (detector == "fahrenheit") {
        var far = (temp * 9 / 5) + 32;
        document.querySelector("#deg").innerHTML = Math.round(far) + "&deg;F";
        var farmin = (mintemp * 9 / 5) + 32;
        document.querySelector("#min").innerHTML = Math.round(farmin) + "&deg;F";
        var farmax = (maxtemp * 9 / 5) + 32;
        document.querySelector("#max").innerHTML = "|" + Math.round(farmax) + "&deg;F";
    }

    else {
        document.querySelector("deg").innerHTML = Math.round(temp) + "&deg;C";
        document.querySelector("min").innerHTML = Math.round(temp-min) + "&deg;C";
        document.querySelector("max").innerHTML = Math.round(temp-max) + "&deg;C";

    }
}