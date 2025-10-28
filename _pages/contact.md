---
permalink: /contact/
title: "Contact"
author_profile: false
---
<head>
  <!-- Leaflet CSS & JS -->
  <link rel="stylesheet"
        href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
        integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
        crossorigin=""/>
  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
          integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
          crossorigin=""></script>

  <style>
    #map { height: 330px; }
  </style>
</head>

<!-- Contact details -->
<i class="fa-li fas fa-map-marker fa-2x" aria-hidden="true"></i>
Institut für Sexualwissenschaft und Sexualmedizin<br>
Luisenstraße 57 (Ebene 2, Raum 003)<br>
10117 Berlin<br>
<a href="https://www.openstreetmap.org/directions?from=&to=52.5256527%2C13.3767302"
   target="_blank" rel="noopener noreferrer">
  Open in OSM
</a><br>
Plus‑code: G9GH+7P Berlin<br>
Email: <a href="mailto:project-veranda@protonmail.com">project-veranda@protonmail.com</a>

<!-- Map -->
<i class="fa-li fas fa-compass fa-2x" aria-hidden="true"></i>
<div id="map"></div>

<script>
  // ----- NEW COORDINATES -------------------------------------------------
  const loc = [52.5256527, 13.3767302];   // Latitude, Longitude

  // Initialise the map centred on the new location
  const map = L.map('map').setView(loc, 16);

  // Add the OpenStreetMap tile layer
  L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
  }).addTo(map);

  // Create a marker at the exact point
  const marker = L.marker(loc).addTo(map);

  // Popup with the human‑readable address (helps confirm the location)
  const addressHtml = `
    <strong>Institut für Sexualwissenschaft und Sexualmedizin</strong><br>
    Luisenstraße 57 (Ebene 2, Raum 003)<br>
    10117 Berlin
  `;
  marker.bindPopup(addressHtml).openPopup();   // Opens automatically on load
</script>
