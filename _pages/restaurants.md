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
    </style>    <meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta http-equiv="X-UA-Compatible" content="ie=edge">
<!--https://code.jquery.com/jquery-3.3.1.js
    https://code.jquery.com/jquery-3.3.1.min.js -->
<title>Near Restaurant</title>
     	<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:300,400"><!-- Google web font "Open Sans" -->
<p id="demo"></p>
                        <input type="text" id="localtion" name="localtion" placeholder="Search Locations..." required="">
<button type="submit" onclick="codeAddress()">Search</button>
<button title="Click here for current location" onclick="getLocation()" type="submit">See nearby</button>

<hr>