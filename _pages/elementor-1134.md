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
			<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        input[type=text], select, textarea {
            width: 50%;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 12px;
            resize: vertical;
        }
        .button {
            background-color: #008CBA;
            border: none;
            color: white;
            padding: 11px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            cursor: pointer;
        }
        .button1 {
            border-radius: 12px;
            width: 150px;
        }
    </style>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <!--https://code.jquery.com/jquery-3.3.1.js
    https://code.jquery.com/jquery-3.3.1.min.js -->
    <title>Near Restaurant</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:300,400"><!-- Google web font "Open Sans" -->
</head>
<body>
    <p id="demo"></p>
                        <input type="text" id="localtion" name="localtion" placeholder="Search Locations..." required />
                        <button type="submit" onclick="codeAddress()">Search</button>
                        <button onclick="getLocation()" type="submit">See nearby</button>
                <br />
                    <label for="placeType" style="font-family:Tahoma;font-size:20px;color:black">Where would you like to eat today ?</label>
                    <br>
                    <br>
                    <input type="radio" name="foodType" value='bakery'  onchange="initialize()" />Bakery
                    <input style="font-family:Tahoma;padding-left:5px" type="radio" name='foodType' value="cafe" onchange="initialize()" />Cafe
                    <input style="font-family:Tahoma" type="radio" name="foodType" value='meal_delivery' onchange="initialize()"/>Delivered Meal
                    <input style="font-family:Tahoma" type="radio" name="foodType" value='meal_takeaway' onchange="initialize()" />Takeaway Meal
                    <input style="font-family:Tahoma" type="radio" name="foodType" checked="checked" value='restaurant' onchange="initialize()" />Restaurant
                    <input style="font-family:Tahoma" type="radio" name="foodType" value='shopping_mall' onchange="initialize()" />Shopping Mall
                    <input style="font-family:Tahoma" type="radio" name="foodType" value='supermarket' onchange="initialize()" />Supermarket
                <br />
                <hr>
</body>
</html>