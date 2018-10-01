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
<!Doctype html>
<html lang="en">
<head>
	<meta charset="utf-8" />
	<title>Current Pollen Conditions</title>
</head>
<body onload="getPollenCounts()">
	<style>
        .pollenLables{
            font-family:Tahoma;
            font-size:30px;
            font-weight:bolder;
            color:black;
            text-align: center;
        }
        .pollenFields{
            font-family:Tahoma;
            color:navy;
            font-size:15px;
            font-weight:bold;
            color:black;
        }
        .pollenValues{
            padding-left:50px;
            color:navy;
            font-size:15px;
         }
    </style>
	<p style="text-align:center;font-size:30px;font-family:Tahoma;color:black;font-weight:bolder">Current Pollen conditions in Melbourne</p>
	<!--Tree Pollen Column Start-->
	<img src="https://i.pinimg.com/originals/0d/fd/8f/0dfd8f4fb49167f674907aa8c97ba34c.png" style="height:100px" alt="tree" />
	<p> Tree</p>
	<p>LevelFetching..</p>
	<p>CategoryFetching..</p>
	<!--Tree Pollen Column End-->
	<!--Grass Pollen Column Start-->
	<img src="http://www.clker.com/cliparts/n/3/s/i/6/6/green-grass-md.png" style="height:100px" alt="wood"/>
	<p >Grass</p>
	<p>LevelFetching..</p>
	<p>CategoryFetching..</p>
	<!--Grass Pollen Column End-->
	<!--Mold Pollen Column Start-->
	<img src="https://static.wixstatic.com/media/f108b3_a74dd059b9c44de2b52ba842e944a6ac~mv2.png/v1/fill/w_200,h_200,al_c,q_80,usm_0.66_1.00_0.01/f108b3_a74dd059b9c44de2b52ba842e944a6ac~mv2.webp" style="height:100px;" alt="mold"/>
	<p >Mold</p>
	<p>LevelFetching..</p>
	<p>CategoryFetching..</p>
	<!--Mold Pollen Column Start-->
	<!--Ragweed Pollen Column Start-->
	<img src="https://openclipart.org/image/2400px/svg_to_png/274424/GiantRagweed.png" style="height:100px;" alt="ragweed" />
	<p>Ragweed  </p>
	<p>LevelFetching..</p>
	<p>CategoryFetching..</p>
	<!--Ragweed Pollen Column Start-->
	<!--Air Quality Start-->
	Overall Air Quality
	<img src="https://mbtskoudsalg.com/images/air-clipart-transparent-background-wind-7.png" style="height:100px;" alt="air"/>
	<p>LevelFetching..</p>
	<p>CategoryFetching..</p>
	<!--Air Quality End-->
	<!--Level Category Description-->
	<pre><strong style="padding-left:15px">Level :</strong>&nbsp;Value associated with the category. These values range from 1 to 6, with 1 implying good conditions and 6 implying hazardous conditions.<br /><br /><strong style="padding-left:15px">Category :</strong>&nbsp;Category of the pollution. Low, High, Good, Moderate, Unhealthy, Hazardous</pre>        
	<!--Level Category Description-->
	<!--Accuweather Logo-->
	<p style="text-align: center;">Powered by:</strong></p>
	<a href="https://developer.accuweather.com/"><img src="http://apidev.accuweather.com/developers/Media/Default/logo//awx-logo-orange.png" width="200" alt="logoaccu"></a>
	<!--Accuweather Logo-->
</body>
</html>