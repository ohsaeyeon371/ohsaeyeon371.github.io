<!-- 지도 api
<!DOCTYPE html>
<html>
<head>
  <title>OpenStreetMap Example</title>
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" />
  <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>
  <style>
    #map {
      height: 400px;
      width: 100%;
    }
  </style>
</head>
<body>
  <h3>OpenStreetMap Example</h3>
  <div id="map"></div>

  <script>
    var map = L.map('map').setView([37.5665, 126.9780], 13); // 서울 중심
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 19,
    }).addTo(map);

    var marker = L.marker([37.5665, 126.9780]).addTo(map);
  </script>
</body>
</html> -->


---
title: "My Map"
---

여기에 OpenStreetMap 지도가 표시됩니다.

{{< osm lat="37.5665" lng="126.9780" zoom="13" >}}
