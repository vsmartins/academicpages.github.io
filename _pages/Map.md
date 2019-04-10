<!DOCTYPE html>

<html>

<head>

<title>Leaflet Web Map</title>
<link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.css" />
<script src="http://cdn.leafletjs.com/leaflet-0.7.3/leaflet.js"></script>
<style>

#map {
width: 960px;
height: 500px;
}

</style>

</head>

<body>

<div id="map"></div>

<script>
    
    var map = L.map('map',{
    center: [43.64701, -79.39425],
    zoom: 15
    });

    L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="http://osm.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);
</script>

</body>

</html>
