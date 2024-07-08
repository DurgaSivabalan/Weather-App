
# Weather App

CSS CODE FILE:

*{
    box-sizing:border-box;
}
body{
    font-family:sans-serif;
    background-color: violet;
    color:aliceblue;
}
.nav-bar img{
margin:20px 0 0 80px;
cursor:pointer;
}
.nav{
    margin:-50px 0 0 48%;
}
.nav li{
    display:inline;
    margin:0 0 0 60px;
    font-size:18px;
    cursor:pointer;
}
.nav .button{
    border:none;
    outline:none;
    border-radius: 5px;
    padding:10px 30px;
    font-size: 18px;
    color:#fff;
    background-color: linear-gradient(90deg,#00b1f7,#0088e1);
    cursor:pointer;
}
.container
{
    display:flex;
    justify-content:space-around;
    margin-top:6%;
}
.interface .h1{
font-weight:normal;
letter-spacing:2px;
word-spacing:3px;
font-size: 35px;
}
.news{
    margin:50px 0 50px 0;
}
.interface p{
    letter-spacing:5px;
    font-size:20px;
}
.material-icons{
    position:relative;
    margin:18px 0 0 30px;
}
.interface.input{
    border:none;
    outline:none;
    padding:20px 100px;
    border-radius: 5px 0 05px;
    font-size:20px ;
    margin-bottom:5px ;
background-color:violet;
letter-spacing:1px;
color:#fff;
}
::placeholder{
    font-size: 20px;
    color:#f1f1f1;
    letter-spacing: 1px;
    word-spacing:1px;
}
.interface.button
{
    border:none;
    outline:none;
    margin-left:10px;
    padding:20px 50px;
    border-radius:0 5px 5px 0;
    font-size:20px;
color:#f1f1f1;
background-color: linear-gradient(to right,violet,#00b1f7);
cursor:pointer;
}
.interface.button:hover{
    background-color: linear-gradient(to right,#00b1f7 #0088e1)
}
.info{
 background-color: violet;
 width:  400px;
 height:500px;
 margin-top: -25px;
 box-shadow:2px 3px 10px #000;
}
.info.header{
    background-color:violet;
    padding: 20px;
    display:flex;

}
.header.h1{
    margin:30px;
}
.header.h3{
    margin:50px;
    text-indent: 20px;
    text-align: center;
}
.header h1::before{
    content:'';
    position:absolute;
    top: 150px;
margin-left:25px;
background-image: url('C:\Users\durga\OneDrive\Desktop\WeatherApp\images\cloud_29dp_5F6368_FILL0_wght400_GRAD0_opsz24.png');
background-size: contain;
background-repeat: no-repeat;
width:100px;
height:100px;

}
.info.report{
    text-align:center;
}
#description{
    font-size: 20px;
    text-transform: capitalize;
    position: relative;
    top:-50px;
    text-shadow: 1px 1px 2px black;

}
.info.output{
    display: inline-flex;
    justify-content: center;;
}
.digit{
    margin-left: 100px;

}
.digit.h1{
    text-shadow: 1px 1px 3px #000;
}
.digit.span{
    font-size: 18px;
}
.list-info{
    margin:10px 150px;
}
#wind::before{
    content:'';
    width:30px;
    height: 30px;
    position: absolute;
    right:200px;
    margin-top:200px;
    background-image:url('C:\Users\durga\OneDrive\Desktop\WeatherApp\images\temp_preferences_eco_48dp_5F6368_FILL0_wght400_GRAD0_opsz48.png');
    background-size: contain;
}
#humidity::before{
    content:'';
    width:30px;
    height: 30px;
    position: absolute;
    right:200px;
    margin-top:-5px;
    background-image: url('C:\Users\durga\OneDrive\Desktop\WeatherApp\images\thermometer_48dp_5F6368_FILL0_wght400_GRAD0_opsz48.png');
}
.convertor{
    text-align: center;
    margin-top: 20px;
    font-size: 20px;
    cursor:pointer;
}