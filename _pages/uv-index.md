---
ID: 556
post_title: 'Today&#8217;s UV Index'
author: aashish
post_excerpt: ""
layout: page
permalink: https://safeworkmel.com/uv-index/
published: true
post_date: 2018-09-11 15:40:58
---
<!-- wp:html -->
<!Doctype html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <script src="https://canvasjs.com/assets/script/canvasjs.min.js"></script>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <title>Current Weather</title>
</head>
<body>

    <style>
        .uvIndexInfo {
            position: relative;
            text-align: center;
        }

        .uvDescLabels {
            font-size: 13pt;
            font-family: arial, helvetica, sans-serif;
        }

        .button {
            background-color: #4CAF50; /* Green */
            border: none;
            color: white;
            padding: 15px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 25px;
            margin: 4px 2px;
            cursor: pointer;
            -webkit-transition-duration: 0.4s; /* Safari */
            transition-duration: 0.4s;
        }

        .button1 {
            box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
        }
    </style>

    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>



    <div class="container" style="height:350px" onload="getCoordinates()">
        <div>
            <img src="https://www.xmple.com/wallpaper/linear-blue-gradient-1920x1080-c2-00ffff-0000cd-a-210-f-14.svg" style="opacity:0.5;width:100%;height:350px" />
            <p style="text-align:center;top:-350px;position:relative;font-size:38px;font-family:Arial;font-weight:bolder">Current weather conditions in Melbourne</p>

            <div class="row" style="text-align:center;position:relative;top:-350px">


                <div class="col-md-4" style="text-align:center">

                    <img src="https://clipart.info/images/ccovers/1486149501Sunshine-free-sun-clipart-public-domain-sun-clip-art-images-and-3.png" style="height:100px;width:100px" />
                    <p style="text-align:center; font-family:Arial;font-weight:bold;font-size:30px">UV Index</p>
                    <p id="uvIndex" style="color:black;font-weight:bold;text-align:center;height:50px;font-family:Arial;font-size:30px">Fetching..</p>

                </div>


                <div class="col-md-4" style="text-align:center">

                    <img src="http://www.transparentpng.com/download/temperature/temperature-png-transparent-pictures-2.png" style="height:100px;width:100px" />
                    <p style="text-align:center;font-family:Arial;font-weight:bold;font-size:30px">Temperature</p>
                    <p id="temperature" style="text-align:center;font-weight:bold;height:50px;font-family:Arial;font-size:30px;color:black">Fetching..</p>

                </div>



                <div class="col-md-4" style="text-align:center">

                    <img src="https://cdn4.iconfinder.com/data/icons/handdrawn-weather-forecast/500/Windy-512.png" style="height:100px;width:100px" />
                    <p style="text-align:center;font-family:Arial;font-weight:bold;font-size:30px">Wind Speed</p>
                    <p id="windSpeed" style="text-align:center;font-weight:bold;height:50px;font-family:Arial;font-size:30px;color:black">Fetching..</p>

                </div>

                <p id="summary" style="color:gray;text-align:center;font-family:Arial ;font-size:40px;font-weight:bolder">Fetching..</p>
            </div>

        </div>
    </div>

    <div id="chartContainer" style="height: 900px; width: 100%"></div>
    <div style="position:relative;top:-460px; font-family:Arial;font-weight:bolder;font-size:50px;text-align:center"> UV Index Chart </div>
    <div style="position:relative;top:-480px; font-family:Arial;font-weight:bolder;font-size:20px;text-align:center"> Click on the colors to know more</div>
    
    <div style="position:relative;top:-450px;text-align:center">
        <div id="tipsDis" style="font-size:30px">
        </div>
        <button class="button botton1" onclick="newTip()">Do U Know ?</button>
    </div>

    <div id="#00ff99" style="position:relative;top:-450px;text-align:center;display:none">
        <h1 style="font-family:Arial;color:gray;font-weight:bold">UV Index 0 - 2</h1>
        <h4 class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;<span style="color: #00ff99;"><strong>LOW</strong></span></span></h4>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> More than 60 Minutes</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen SPF 30-50 (waterproof, broad sprectrum)</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Portable water bottle to stay hydrated, Sun protective hat UPF 50+</span></div>
        <div class="uvIndexInfo">&nbsp;</div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: 'arial black', 'avant garde';">When UV Index is Low, not much protection is required. </span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: 'arial black', 'avant garde';">But one may have a sensitive skin and still might need protection. </span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: 'arial black', 'avant garde';">Take all the basic prevention measures and </span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: 'arial black', 'avant garde';">seek shade whenever possible after every 45 minutes.</span></div>
    </div>
    <div id="#f4e242" style="position:relative;top:-450px;text-align:center;display:none">
        <h1 style="font-family: Arial; color: gray; font-weight: bold;">UV Index 3 - 5</h1>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="color: #4d4d4d;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;</span><span style="color: #f4e242;"><strong>Moderate</strong></span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> Approximately 30 Minutes</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen SPF 30-50+ (waterproof, broad sprectrum)</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;<span style="line-height: 107%;">Portable water bottle to stay hydrated, Sun protective hat UPF 50+, EPF 9 sunglasses</span></span></div>
        <div class="uvIndexInfo">&nbsp;</div>
        <div class="uvIndexInfo"><span style="font-family: 'arial black', 'avant garde'; font-size: 13pt;">UV Index may not cause much harm but still can cause harm.</span></div>
        <div class="uvIndexInfo"><span style="font-family: 'arial black', 'avant garde'; font-size: 13pt;">Try seeking shade every 20 minutes and keep your body parts covered. </span></div>
        <div class="uvIndexInfo"><span style="font-family: 'arial black', 'avant garde'; font-size: 13pt;">Reapply Sunscreen every 2 hours.</span></div>
    </div>
    <div id="#ffd505" style="position:relative;top:-450px;text-align:center;display:none">
        <h1 style="font-family:Arial;color:gray;font-weight:bold">UV Index 6 - 7</h1>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="color: #4d4d4d;"><strong>Danger Category&nbsp; :&nbsp;</strong></span>&nbsp;<span style="color: #ffd505;"><strong>High</strong></span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> Less than 30 Minutes</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;</strong>Sunscreen&nbsp;</span><span style="line-height: 107%;">(waterproof, broad spectrum) SPF 100+), </span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="line-height: 107%;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Sun protective hat UPF 50+, UV protection sun glasses EPF 9</span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:&nbsp;</strong><span style="line-height: 107%;">Portable water bottle to stay hydrated, umbrella</span></span></div>
        <div class="uvIndexInfo">&nbsp;</div>
        <div class="uvIndexInfo"><span style="font-family: 'arial black', 'avant garde'; font-size: 13pt;">Seek shade during the midday hours, reapply the Sunscreen every hours and stay hydrated</span></div>
    </div>
    <div id="#ff7905" style="position:relative;top:-450px;text-align:center;display:none">
        <h1 style="font-family:Arial;color:gray;font-weight:bold">UV Index 8 - 10</h1>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong><span style="color: #4d4d4d;">Danger Category&nbsp; :</span>&nbsp;</strong>&nbsp;<span style="color: #ff7905;"><strong>Very High</strong></span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> Approximately 20 Minutes</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;</strong></span></span>Sunscreen (waterproof, broad spectrum) SPF 100+),</span><br /><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="line-height: 107%;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Sun protective hat UPF 50+, UV protection sun glasses EPF 10</span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:&nbsp;</strong></span>Portable water bottle to stay hydrated, umbrella, Sun protection clothing UPF50+</span></div>
        <div class="uvIndexInfo"><span style="font-family: 'arial black', 'avant garde';"><strong><span style="font-size: 13pt; color: #4d4d4d;">If possible, avoid going outside during midday hours. Seek shade whenever possible.</span></strong></span></div>
    </div>
    <div id="#ff0505" style="position:relative;top:-450px;text-align:center;display:none">
        <h1 style="font-family:Arial;color:gray;font-weight:bold">UV Index 11+</h1>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="color: #999999;"><strong><span style="color: #4d4d4d;">Danger Category&nbsp; :</span>&nbsp;</strong></span>&nbsp;<span style="color: #ff7905;"><strong>Extreme</strong></span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Less than 20 Minutes</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:&nbsp;</strong>Sunscreen&nbsp;</span></span></span><span style="line-height: 107%;">(waterproof, broad spectrum) SPF 100+), </span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="line-height: 107%;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Sun protective hat UPF 50+, UV protection sun glasses EPF 10</span></span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:&nbsp;</strong></span></span>Portable water bottle to stay hydrated, umbrella,</span></div>
        <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: arial, helvetica, sans-serif; color: #4d4d4d;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; sun protection clothing UPF50+, reflective gloves</span></div>
        <div class="uvIndexInfo"><span style="font-size: 14pt; font-family: 'arial black', 'avant garde'; color: #000000;"><strong>You must completely avoid going out when UV Index is Extreme.</strong></span></div>
        <div class="uvIndexInfo"><span style="font-size: 14pt; font-family: 'arial black', 'avant garde'; color: #000000;"><strong>Seek shade whenever possible if staying outside</strong></span></div>
 	</div>
	
	        <div class="row" style="position:relative;top:-380px;width:100%;text-align:center">
            <p style="text-align: center;"><strong><span style="font-size: 16pt; font-family: Arial">Powered by</span></strong></p>
            <a href="https://openweathermap.org/api"><img src="https://assets.planet.com/partners/logos/openweathermap.png" width="100" height="100"></a>
            <a href="https://darksky.net/dev"><img src="https://www.vectorlogo.zone/logos/darksky/darksky-card.png" width="200" height="100"></a>
        </div>

	<script>
        var lon;
        var lat;

        function getCoordinates() {

            $.ajax({
                url: 'https://api.openweathermap.org/data/2.5/weather?zip=' + "3001" + ",au&units=metric" +
                    "&APPID=2122a4167828b10f63dc38e69a7cae9b",
                type: "GET",
                async: false,
                dataType: "jsonp",
                success: function (data) {
                    lon = data.coord.lon;
                    lat = data.coord.lat;
                    getUVdata(lon, lat);
                }
            });
        }
        function getUVdata(lon, lat) {
            $.ajax({
                url: 'https://api.darksky.net/forecast/606a5e9b7758dfc86513a60e874c87c5/' + lat + "," + lon + "?units=si",
                type: "GET",
                async: false,
                dataType: "jsonp",
                success: function (uvdata) {
                    var uvI = uvdata.currently.uvIndex;
                    $("#uvIndex").html(uvI);

                    var temp = uvdata.currently.temperature + '&deg';
                    $("#temperature").html(temp);

                    var wind = uvdata.currently.windSpeed;
                    $("#windSpeed").html(wind);

                    var summ = uvdata.currently.summary;
                    $("#summary").html(summ);
                }
            });
        }
        $(document).ready(function () {
            getCoordinates()
        });

    </script>
<script>
        var chart = new CanvasJS.Chart("chartContainer",
            {

                data: [
                    {
                        type: "doughnut",
                        innerRadius: "0%",
                        indexLabelPlacement: "inside",
                        toolTipContent: "<br/> {x}: {label} ",
                        showInLegend: false,
                        click: uv1,
                        dataPoints: [
                            { y: 3, label: "UV 0 - 2", color: "#00ff99", },
                            { y: 3, label: "UV 3 - 5", color: "#f4e242" },
                            { y: 2, label: "UV 6 - 7", color: "#ffd505" },
                            { y: 3, label: "UV 8 -10", color: "#ff7905" },
                            { y: 1, label: "UV 11+", color: "#ff0505" }
                        ]
                    }
                ]
            });

        convertToHalfPie(chart);
        chart.render();

        function uv1(e) {
            var x = document.getElementById(e.dataPoint.color);

            if (x.style.display == "none") {
                x.style.display = "block";
            } else {
                x.style.display = "none";
            }
        }

        function convertToHalfPie(chart) {
            var sum = 0;
            var dataPoints = chart.options.data[0].dataPoints;

            for (var i = 0; i < dataPoints.length; i++) {
                sum += dataPoints[i].y;
            }

            dataPoints.splice(0, 0, { y: sum, color: "transparent", toolTipContent: null });
        }</script>

	<script>
        var facts = [
            'Two in three Australians will be diagnosed with skin cancer by the age of 70',
            'More than 2,000 Australians die from skin cancer each year',
            'Australia has one of the highest rates of skin cancer in the world',
            'The incidence of treatments for basal and squamous cell carcinomas is more than five times the incidence of all other cancers combined',
            'Medicare records show there were over 900,000 treatments for squamous and basal cell carcinoma skin cancers in 2016 that more than 2,500 skin cancer treatments every day.',
            'The cost to the health system of these skin cancers alone is estimated to be more than $700 million annually',
            'In 2015, 379 Victorians died from skin cancer, 1.5 times the Victorian road toll that year',
            'It is estimated that approximately 200 melanomas and 34,000 other skin cancer types per year are caused by occupational exposures in Australia',
            'SPF30 filters 96.7% of UV radiation with 1/30th (3.3%) of UV reaching the skin. SPF50 filters 98% of UV radiation with 1/50th (2%) reaching the skin.',
            'Applying the sunscreen at least 20 minutes before going outside',
            'Melanoma represents 2% of all skin cancers, but causes 75% of skin cancer deaths'
        ]

        function newTip() {
            var randomNumber = Math.floor(Math.random() * (facts.length));
            document.getElementById('tipsDis').innerHTML = facts[randomNumber];

        }


    </script>



</body>

</html>
<!-- /wp:html -->