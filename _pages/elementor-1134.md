---
ID: 1134
post_title: 'Elementor #1134'
author: aashish
post_excerpt: ""
layout: page
permalink: https://safeworkmel.com/elementor-1134/
published: true
post_date: 2018-10-01 19:29:34
---
<!-- wp:fl-builder/layout /-->

<p><br>
<br>
</p>
<style>
        input[type=text], select, textarea {<br />
            width: 50%;<br />
            padding: 20px;<br />
            border: 1px solid #ccc;<br />
            border-radius: 12px;<br />
            resize: vertical;<br />
        }<br />
        .button {<br />
            background-color: #008CBA;<br />
            border: none;<br />
            color: white;<br />
            padding: 11px;<br />
            text-align: center;<br />
            text-decoration: none;<br />
            display: inline-block;<br />
            font-size: 16px;<br />
            margin: 4px 2px;<br />
            cursor: pointer;<br />
        }<br />
        .button1 {<br />
            border-radius: 12px;<br />
            width: 150px;<br />
        }<br />
    </style>
<p>    <meta charset="UTF-8"><br>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"><br>
    <meta http-equiv="X-UA-Compatible" content="ie=edge"><br>
    <!--https://code.jquery.com/jquery-3.3.1.js
    https://code.jquery.com/jquery-3.3.1.min.js --><br>
    <title>Near Restaurant</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:300,400"><!-- Google web font "Open Sans" --><br>
<br>

    </p><p id="demo"></p>
<p>                        <input type="text" id="localtion" name="localtion" placeholder="Search Locations..." required=""><br>
                        <button type="submit" onclick="codeAddress()">Search</button><br>
                        <button onclick="getLocation()" type="submit">See nearby</button><br>
                <br>
                    <label for="placeType" style="font-family:Tahoma;font-size:20px;color:black">Where would you like to eat today ?</label></p>
<p>                    <input type="radio" name="foodType" value="bakery" onchange="initialize()">Bakery<br>
                    <input style="font-family:Tahoma;padding-left:5px" type="radio" name="foodType" value="cafe" onchange="initialize()">Cafe<br>
                    <input style="font-family:Tahoma" type="radio" name="foodType" value="meal_delivery" onchange="initialize()">Delivered Meal<br>
                    <input style="font-family:Tahoma" type="radio" name="foodType" value="meal_takeaway" onchange="initialize()">Takeaway Meal<br>
                    <input style="font-family:Tahoma" type="radio" name="foodType" checked="checked" value="restaurant" onchange="initialize()">Restaurant<br>
                    <input style="font-family:Tahoma" type="radio" name="foodType" value="shopping_mall" onchange="initialize()">Shopping Mall<br>
                    <input style="font-family:Tahoma" type="radio" name="foodType" value="supermarket" onchange="initialize()">Supermarket<br>
                </p>
<hr>
<br>
<p></p>