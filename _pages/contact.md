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
    /* Height for the map container */
    #map { height: 330px; }
  </style>
</head>

<!-- ==================== CONTACT DETAILS ==================== -->
<i class="fa-li fas fa-map-marker fa-2x" aria-hidden="true"></i>
<strong>Prof. Dr.-Ing Maija Poikela</strong><br>
AG Health Data Privacy<br>
Rahel‑Hirsch‑Center for Translational Medicine<br>
Luisenstraße 65 (Ebene 2, Raum 003)<br>
Charitéplatz 1, 10117 Berlin<br>
<a href="https://www.openstreetmap.org/directions?from=&to=52.5268647%2C13.3787751"
   target="_blank" rel="noopener noreferrer">
  Open in OpenStreetMap
</a><br>
Plus‑code: G9GH+7P Berlin<br>
Email: <a href="mailto:project-veranda@protonmail.com">project-veranda@protonmail.com</a>

<!-- ==================== MAP ==================== -->
<i class="fa-li fas fa-compass fa-2x" aria-hidden="true"></i>
<div id="map"></div>

<script>
  // ----- UPDATED COORDINATES (Rahel‑Hirsch‑Center) -----
  const loc = [52.5268647, 13.3787751];   // latitude, longitude

  // Initialise the map centred on the new location
  const map = L.map('map').setView(loc, 16);

  // Load OpenStreetMap tiles
  L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
  }).addTo(map);

  // Marker at the exact point
  const marker = L.marker(loc).addTo(map);

  // Popup with the full address (helps confirm the spot)
  const addressHtml = `
    <strong>Prof. Dr.-Ing Maija Poikela</strong><br>
    AG Health Data Privacy<br>
    Rahel‑Hirsch‑Center for Translational Medicine<br>
    Luisenstraße 65 (Ebene 2, Raum 003)<br>
    Charitéplatz 1, 10117 Berlin
  `;
  marker.bindPopup(addressHtml).openPopup();   // opens automatically on page load
</script>
