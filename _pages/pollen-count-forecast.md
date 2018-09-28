---
ID: 657
post_title: Pollen Count Forecast
author: aashish
post_excerpt: ""
layout: page
permalink: >
  https://safeworkmel.com/pollen-count-forecast/
published: true
post_date: 2018-09-13 03:39:26
---
<!-- wp:html -->
<!Doctype html>
<html lang="en">

<head>

	<meta charset="utf-8" />
	<script src="https://canvasjs.com/assets/script/canvasjs.min.js"></script>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
	<title>Current Pollen Conditions</title>

</head>


<body onload="getPollenCounts()">
	<style>
        .pollenLables{
            font-family:Arial;
            font-size:45px;
            font-weight:bolder;
            color:black;
        }

        .pollenFields{
            font-family:Arial;
            font-size:20px;
            font-weight:bold;
            text-align:center;
            color:black;
        }

        .categoryPosition{
            position:relative;
            top:-10px;
        }

        .pollenValues{
            padding-left:50px;
            color:gray;
            font-size:20px;
         }

  
    </style>
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

	<div class="container">

	<img src="https://img00.deviantart.net/047a/i/2012/222/9/8/green_gradient_by_ohsnapjenny-d5an28t.jpg" style="opacity:0.5;width:100%;height:620px" alt="backGreen" />
	<p style="text-align:center;top:-580px;position:relative;font-size:50px;font-family:Arial;font-weight:bolder">Current Pollen conditions in Melbourne</p>
	<div class="row" style="height:290px;text-align:center;position:relative;top:-580px;width:1140px;left:15px">


	<!--Tree Pollen Column Start-->
	<div class="col-lg-3">
	<img src="https://i.pinimg.com/originals/0d/fd/8f/0dfd8f4fb49167f674907aa8c97ba34c.png" style="height:140px;width:110px" alt="tree" />
	<div class="row pollenLables" style="padding-left:100px"> Tree</div>
	<p class="pollenFields">Level<span id="treePollen" class="pollenValues">Fetching..</span></p>
	<p class="pollenFields categoryPosition">Category<span id="treePollenCategory" class="pollenValues" style="padding-left:15px">Fetching..</span></p>
	</div>
	<!--Tree Pollen Column End-->

	<!--Grass Pollen Column Start-->
	<div class="col-lg-3" style="height:290px">
	<img src="http://www.clker.com/cliparts/n/3/s/i/6/6/green-grass-md.png" style="height:140px;width:190px" alt="wood"/>
	<div class="row pollenLables" style="padding-left:70px">Grass</div>
	<p class="pollenFields">Level<span id="grassPollen" class="pollenValues">Fetching..</span></p>
	<p class="pollenFields categoryPosition">Category<span id="grassPollenCategory" class="pollenValues" style="padding-left:15px">Fetching..</span></p>
	</div>
	<!--Grass Pollen Column End-->


	<!--Mold Pollen Column Start-->
	<div class="col-lg-3" style="height:290px">
	<img src="https://static.wixstatic.com/media/f108b3_a74dd059b9c44de2b52ba842e944a6ac~mv2.png/v1/fill/w_200,h_200,al_c,q_80,usm_0.66_1.00_0.01/f108b3_a74dd059b9c44de2b52ba842e944a6ac~mv2.webp" style="height:140px;width:140px" alt="mold"/>
	<div class="row pollenLables" style="padding-left:90px">Mold</div>
	<p class="pollenFields">Level<span id="moldPollen" class="pollenValues">Fetching..</span></p>
	<p class="pollenFields categoryPosition">Category<span id="moldPollenCategory" class="pollenValues" style="padding-left:15px">Fetching..</span></p>
	</div>
	<!--Mold Pollen Column Start-->


	<!--Ragweed Pollen Column Start-->
	<div class="col-lg-3" style="height:290px">
	<img src="https://openclipart.org/image/2400px/svg_to_png/274424/GiantRagweed.png" style="height:140px;width:140px" alt="ragweed" />
	<div class="row pollenLables" style="padding-left:40px">Ragweed  </div>
	<p class="pollenFields">Level<span id="ragweedPollen" class="pollenValues">Fetching..</span></p>
	<p class="pollenFields categoryPosition">Category<span id="ragweedPollenCategory" class="pollenValues" style="padding-left:15px">Fetching..</span></p>
	</div>
	<!--Ragweed Pollen Column Start-->

	</div>

	<!--Air Quality Start-->
	<div class="row" style="text-align:center;position:relative;top:-580px">
	<div class="pollenLables">Overall Air Quality</div>
	<div class="col-lg-6" style="text-align:right">
	<img src="https://mbtskoudsalg.com/images/air-clipart-transparent-background-wind-7.png" style="height:140px;width:140px" alt="air"/>
	</div>

	<div class="col-lg-3" style="padding-top:35px">
	<p class="pollenFields">Level<span id="airQuality" class="pollenValues">Fetching..</span></p>
	<p class="pollenFields categoryPosition">Category<span id="airQualityCategory" class="pollenValues" style="padding-left:15px">Fetching..</span></p>
	</div>
	</div>
	<!--Air Quality End-->


	<!--Level Category Description-->
	<div class="row" style="position:relative;top:-590px;left:15px;width:1140px">
	<pre><span style="font-family: calibri, sans-serif; font-size: 13pt;"><strong>Level :</strong>&nbsp;Value associated with the category. These values range from 1 to 6, with 1 implying good conditions and 6 implying hazardous conditions.</span><br /><br /><span style="font-family: calibri, sans-serif; font-size: 13pt;"><strong>Category :</strong>&nbsp;Category of the pollution. Low, High, Good, Moderate, Unhealthy, Hazardous)</span></pre>        </div>
	<!--Level Category Description-->


	<!--Accuweather Logo-->
	<div class="row" style="position:relative;top:-570px;left:15px;width:1140px;text-align:center">
	<p style="text-align: center;"><strong><span style="font-size: 12pt; font-family: arial, helvetica, sans-serif;">Powered by</span></strong></p>
	<a href="https://developer.accuweather.com/"><img src="http://apidev.accuweather.com/developers/Media/Default/logo//awx-logo-orange.png" width="350" height="50" alt="logoaccu"></a>
	</div>
	<!--Accuweather Logo-->

	</div> 
		
	<script>

        function getPollenCounts() {

            $.ajax({
                url: 'https://dataservice.accuweather.com/forecasts/v1/daily/1day/26216?apikey=G3uSRBti3IEb6f7gVAylEh3B7KAlB6PN&details=true',
                type: "GET",
                async: false,
                dataType: "jsonp",
                success: function (data) {
                    var treePol = data.DailyForecasts[0].AirAndPollen[4].CategoryValue;
                    $("#treePollen").html(treePol);
                    var treePolCat = data.DailyForecasts[0].AirAndPollen[4].Category;
                    $("#treePollenCategory").html(treePolCat);

                    var grassPol = data.DailyForecasts[0].AirAndPollen[1].CategoryValue;
                    $("#grassPollen").html(grassPol);
                    var grassPolCat = data.DailyForecasts[0].AirAndPollen[1].Category;
                    $("#grassPollenCategory").html(grassPolCat);

                    var moldPol = data.DailyForecasts[0].AirAndPollen[2].CategoryValue;
                    $("#moldPollen").html(moldPol);
                    var moldPolCat = data.DailyForecasts[0].AirAndPollen[2].Category;
                    $("#moldPollenCategory").html(moldPolCat);

                    var ragweedPol = data.DailyForecasts[0].AirAndPollen[3].CategoryValue;
                    $("#ragweedPollen").html(ragweedPol);
                    var ragweedPolCat = data.DailyForecasts[0].AirAndPollen[3].Category;
                    $("#ragweedPollenCategory").html(ragweedPolCat);

                    var airQual = data.DailyForecasts[0].AirAndPollen[0].Value;
                    $("#airQuality").html(airQual);
                    var airQualCat = data.DailyForecasts[0].AirAndPollen[0].CategoryValue;
                    $("#airQualityCategory").html(airQualCat);

                }
            });
        }

        $(document).ready(function () {
            getPollenCounts()
        });
       
    </script>

</body>


</html>
<!-- /wp:html -->