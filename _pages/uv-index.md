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
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <script src="https://canvasjs.com/assets/script/canvasjs.min.js"></script>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
</head>
<body>
    <style>

        .uvIndexInfo {
            color: white;
            font-family: Tahoma;
        }

        .uvSuggestion {
            font-family: Calibri;
            font-size: 30px;
            font-weight: bolder;
            color: black;
            padding-right: 10px;
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

        .uvIndex02Gradient {
            background: #24C6DC; /* fallback for old browsers */
            background: -webkit-linear-gradient(to right, #514A9D, #24C6DC); /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to right, #514A9D, #24C6DC); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
        }

        .uvIndex35Gradient {
            background: #F09819; /* fallback for old browsers */
            background: -webkit-linear-gradient(to bottom, #EDDE5D, #F09819); /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to bottom, #EDDE5D, #F09819); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
        }

        .uvIndex68Gradient {
            background: #FDC830; /* fallback for old browsers */
            background: -webkit-linear-gradient(to right, #F37335, #FDC830); /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to right, #F37335, #FDC830); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
        }

        .uvIndex910Gradient {
            background: #FF416C; /* fallback for old browsers */
            background: -webkit-linear-gradient(to bottom, #FF4B2B, #FF416C); /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to bottom, #FF4B2B, #FF416C); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
        }

        .uvIndex11Gradient {
            background: #e52d27; /* fallback for old browsers */
            background: -webkit-linear-gradient(to bottom, #b31217, #e52d27); /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to bottom, #b31217, #e52d27); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
        }
    </style>
    <div class="container" style="width:100%">

        <div style="height:auto">
            <div class="col-lg-4">
                <div class="row" style="text-align:center;padding-top:50px">
                    <div class="col-md-6" style="text-align:center;border:dashed">
                        <img src="https://farm2.staticflickr.com/1970/31086594348_aee6f546be_m.jpg" style="height:150px;width:150px" />
                    </div>
                    <div class="col-sm-1" style="text-align:center">
                        <div class="row" style="padding-top:15px;font-family:Arial;text-align:center;font-weight:bolder;font-size:35px"> UV Index </div>
                        <div id="uvIndex" class="row" style="font-family:Arial;text-align:center;font-weight:bolder;font-size:35px"> Fetching..... </div>
                    </div>
                </div>
                <div class="row" style="text-align:center">
                    <div class="col-md-6" style="text-align:center;border:dashed">
                        <img src="https://farm2.staticflickr.com/1924/43147124940_e5e7338912_o.png" style="height:150px;width:150px" />
                    </div>
                    <div class="col-sm-1" style="text-align:center">
                        <div class="row" style="padding-top:15px;font-family:Arial;text-align:center;font-weight:bolder;font-size:35px"> Temperature </div>
                        <div id="temperature" class="row" style="font-family:Arial;text-align:center;font-weight:bolder;font-size:35px"> Fetching..... </div>
                    </div>
                </div>
            </div>

            <div class="col-lg-8">
                <div id="uvIndex02" class="uvIndex02Gradient" style="text-align:justify;padding-left:10px;padding-bottom:20px;padding-top:10px;display:none">
                    <h1 style="font-family:Arial;color:black;font-weight:900;font-size:50px">UV Index 0 - 2</h1>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <h4 class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;<span style="color: white;"><strong>LOW</strong></span></span></h4>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> More than 60 Minutes</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen SPF 30-50 (waterproof, broad sprectrum)</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Portable water bottle to stay hydrated, Sun protective hat UPF 50+</span></div>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <div class="uvSuggestion">When UV Index is Low, not much protection is required. But one may have a sensitive skin and still might need protection. Take all the basic prevention measures and seek shade whenever possible after every 45 minutes</div>
                    <div class="uvSuggestion"></div>
                </div>

                <div id="uvIndex35" class="uvIndex35Gradient" style="text-align:justify;padding-left:10px;padding-bottom:20px;padding-top:10px;display:none">
                    <h1 style="font-family:Arial;color:black;font-weight:900;font-size:50px">UV Index 3 - 5</h1>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <h4 class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;<span style="color: white;"><strong>MODERATE</strong></span></span></h4>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> Approximately 30 Minutes</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen SPF 30-50+ (waterproof, broad sprectrum)</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;<span style="line-height: 107%;">Portable water bottle to stay hydrated, Sun protective hat UPF 50+, EPF 9 sunglasses</span></span></div>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <div class="uvSuggestion">UV Index may not cause much harm but still can cause harm.</div>
                    <div class="uvSuggestion">Try seeking shade every 20 minutes and keep your body parts covered. </div>
                    <div class="uvSuggestion">Reapply Sunscreen every 2 hours.</div>
                </div>

                <div id="uvIndex68" class="uvIndex68Gradient" style="text-align:justify;padding-left:10px;padding-bottom:20px;padding-top:10px;display:none">
                    <h1 style="font-family:Arial;color:black;font-weight:900;font-size:50px">UV Index 6 - 8</h1>
                    <h4 class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;<span style="color: white;"><strong>HIGH</strong></span></span></h4>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> Less than 30 Minutes</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen (waterproof, broad spectrum) SPF 100+), Sun protective hat UPF 50+, UV protection sun glasses EPF 9</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Portable water bottle to stay hydrated, umbrella</span></div>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <div class="uvSuggestion">Seek shade during the midday hours, reapply the Sunscreen every hours and stay hydrated</div>
                </div>

                <div id="uvIndex910" class="uvIndex910Gradient" style="text-align:justify;padding-left:10px;padding-bottom:20px;padding-top:10px;display:none">
                    <h1 style="font-family:Arial;color:black;font-weight:900;font-size:50px">UV Index 9 - 10</h1>
                    <h4 class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;<span style="color: white;"><strong>VERY HIGH</strong></span></span></h4>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong> Approximately 20 Minutes</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen (waterproof, broad spectrum) SPF 100+),Sun protective hat UPF 50+, UV protection sun glasses EPF 10</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Portable water bottle to stay hydrated, umbrella, Sun protection clothing UPF50+</span></div>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <div class="uvSuggestion">If possible, avoid going outside during midday hours. Seek shade whenever possible.</div>
                </div>

                <div id="uvIndex11" class="uvIndex11Gradient" style="text-align:justify;padding-left:10px;padding-bottom:20px;padding-top:10px;display:none">
                    <h1 style="font-family:Arial;color:black;font-weight:900;font-size:50px">UV Index 11+</h1>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <h4 class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Danger Category&nbsp; :&nbsp;</strong>&nbsp;<span style="color: white;"><strong>EXTREME</strong></span></span></h4>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Sunburn Time&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Less than 20 Minutes</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Must Haves&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;:</strong> Sunscreen (waterproof, broad spectrum) SPF 100+), Sun protective hat UPF 50+, UV protection sun glasses EPF 10</span></div>
                    <div class="uvIndexInfo"><span style="font-size: 13pt; font-family: Tahoma;"><strong>Should Haves&nbsp; &nbsp; &nbsp; &nbsp;:</strong>&nbsp;Portable water bottle to stay hydrated, umbrella,sun protection clothing UPF50+, reflective gloves</span></div>
                    <div class="uvIndexInfo">&nbsp;</div>
                    <div class="uvSuggestion">You must completely avoid going out when UV Index is Extreme. Seek shade whenever possible if staying outside</div>
                </div>
            </div>
            <div class="col-lg-1"></div>
        </div>
    </div>
    <div>&nbsp;</div>
    <div>&nbsp;</div>
    <div class="row" style="text-align:center">
        <p style="font-family:Arial;font-size:25px">Powered By:</p>
        <a href="https://openweathermap.org/api"><img src="https://farm2.staticflickr.com/1943/43156966290_e4b107251b.jpg" width="320" height="30"></a>

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

                    if (uvI == '0' || uvI == '1' || uvI == '2') {
                        uvindex02();
                    }
                    else if (uvI == '3' || uvI == '4' || uvI == '5') {
                        uvindex35();
                    }
                    else if (uvI == '6' || uvI == '7' || uvI == '8') {
                        uvindex68();
                    }
                    else if (uvI == '9' || uvI == '10') {
                        uvindex910();
                    }
                    else if (uvI == '11') {
                        uvindex11();
                    }

                    else {
                        uvindex02();
                    };
                }
            });
        }

        function uvindex02() {

            var x = document.getElementById("uvIndex02");
            if (x.style.display === "none") {
                x.style.display = "block";
            } else {
                x.style.display = "none";
            }

        }
        function uvindex35() {

            var x = document.getElementById("uvIndex35");
            if (x.style.display === "none") {
                x.style.display = "block";
            } else {
                x.style.display = "none";
            }

        }
        function uvindex68() {

            var x = document.getElementById("uvIndex68");
            if (x.style.display === "none") {
                x.style.display = "block";
            } else {
                x.style.display = "none";
            }

        }
        function uvindex910() {

            var x = document.getElementById("uvIndex910");
            if (x.style.display === "none") {
                x.style.display = "block";
            } else {
                x.style.display = "none";
            }

        }
        function uvindex11() {

            var x = document.getElementById("uvIndex11");
            if (x.style.display === "none") {
                x.style.display = "block";
            } else {
                x.style.display = "none";
            }

        }

        $(document).ready(function () {
            getCoordinates()
        });

    </script>

</body>
</html>
<!-- /wp:html -->