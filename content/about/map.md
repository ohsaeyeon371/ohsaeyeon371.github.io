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

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>{{ .Title }}</title>
    {{ partial "head.html" . }}
</head>
<body>
    {{ partial "header.html" . }}

    <main>
        {{ block "main" . }}{{ .Content }}{{ end }}
        
        <!-- Google Maps Script -->
        <div id="map" style="height:400px; width:100%;"></div>
        <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" async defer></script>
        <script>
          function initMap() {
            var location = {lat: 37.5665, lng: 126.9780}; // 서울의 위도와 경도
            var map = new google.maps.Map(document.getElementById('map'), {
              zoom: 12,
              center: location
            });
            var marker = new google.maps.Marker({
              position: location,
              map: map
            });
          }
        </script>
    </main>

    {{ partial "footer.html" . }}
</body>
</html>
