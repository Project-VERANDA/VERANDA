---
permalink: /contact/
title: "Contact"
author_profile: false
---
<head>
 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
     integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
     crossorigin=""/>
 <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
    integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
    crossorigin=""></script>
 <style>
    #map { height: 330px; }
 </style>
</head>

<i class="fa-li fas fa-map-marker fa-2x" aria-hidden="true">
</i>
DFKI
<br>
<a href="https://www.openstreetmap.org/directions?from=&to=52.52422%2C13.34410" target="_blank" rel="noopener noreferrer"> Alt-Moabit 91c<br>10559 Berlin</a> 
<br>
take the elevator to floor 4 and ring the reception bell

<i class="fa-li fas fa-compass fa-2x" aria-hidden="true">
</i>
<div id="map"></div>
<script>
 // old location (TEL):
 // var location = [52.51294, 13.32005] 
 // new location (DFKI):
 var loc = [52.52422, 13.34410]  
 var map = L.map('map').setView(loc, 16);
 L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
 }).addTo(map);
 var marker = L.marker(loc).addTo(map);
</script>