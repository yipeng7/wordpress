---
ID: 704
post_title: Restaurants
author: Yipeng Li
post_excerpt: ""
layout: page
permalink: https://safeworkmel.com/restaurants/
published: true
post_date: 2018-09-13 12:31:15
---
<p style="text-align: center;">Eating places in proximity of current location. Search for a specific location</p>		
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
                <br />
                <hr>
</body>
</html>