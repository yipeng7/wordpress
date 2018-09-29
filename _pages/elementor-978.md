---
ID: 978
post_title: 'Elementor #978'
author: aashish
post_excerpt: ""
layout: page
permalink: https://safeworkmel.com/elementor-978/
published: true
post_date: 2018-09-29 11:18:39
---
<!-- wp:fl-builder/layout /-->		
			<!DOCTYPE html>
<html>
    <head>
    <meta charset="utf-8" />
</head>
<style>
/* The container */
.cont {
    display: block;
    position: relative;
    padding-left: 35px;
    margin-bottom: 12px;
    cursor: pointer;
    font-size: 22px;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
}
/* Hide the browser's default checkbox */
.cont input {
    position: absolute;
    opacity: 0;
    cursor: pointer;
}
/* Create a custom checkbox */
.check {
    position: absolute;
    top: 0;
    left: 0;
    height: 25px;
    width: 25px;
    background-color: #eee;
}
/* On mouse-over, add a grey background color */
.cont:hover input ~ .check {
    background-color: #ccc;
}
/* When the checkbox is checked, add a blue background */
.cont input:checked ~ .check {
    background-color: #2196F3;
}
/* Create the checkmark/indicator (hidden when not checked) */
.check:after {
    content: "";
    position: absolute;
    display: none;
}
/* Show the checkmark when checked */
.cont input:checked ~ .check:after {
    display: block;
}
/* Style the checkmark/indicator */
.cont .check:after {
    left: 9px;
    top: 5px;
    width: 5px;
    height: 10px;
    border: solid white;
    border-width: 0 3px 3px 0;
    -webkit-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    transform: rotate(45deg);
}
</style>
<body>
<h1>Custom Checkboxes</h1>
<label>One
  <input type="checkbox" checked="checked">
</label>
<label>Two
  <input type="checkbox" checked="checked">
</label>
<label>Three
  <input type="checkbox" checked="checked">
</label>
<label>Four
  <input type="checkbox" checked="checked">
</label>
</body>
</html>