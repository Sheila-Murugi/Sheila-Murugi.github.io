<!DOCTYPE html>
<html lang="en">
<body>
    </head>
  <div class="navbar">
    <a class="logo" href="#">Greece Fun Spots!</a>
    <style>
        .navbar {
        background-color: #494747;
        overflow: hidden;
        }
        .navbar .logo {
        float: inline-start;
        font-size: 40px;
        font-weight: bold;
        font-family:  comic sans ms, cursive ; 
        padding: 14px 16px;
        color: rgb(186, 214, 233);
        text-decoration: none;
    }
    
        #description {
      text-align: center;
      margin-top: 10px;
      background: rgb(186, 214, 233);
      padding: 20px;
      font-family:  comic sans ms, cursive ; 
    }
    
    
    </style>
    <div id="description">
                                           <h1>About Greece</h1>
        <p>Greece is a country in southeastern Europe with thousands of islands throughout the Aegean and Ionian seas.</p>
    
          <p>Influential in ancient times, it's often called the cradle of Western civilization. Athens, its capital, retains landmarks including the 5th-century B.C. Acropolis citadel with the Parthenon temple.</p>
          
          <p>Greece is also known for its beaches, from the black sands of Santorini to the party resorts of Mykonos. </p>
          
          <p>Its fascinating culture filled with an abundance of controversial religion makes it an amazing tourist destination.</p>
          <p>If you're a lover of Greek methology, this is definitely the place to be! You might even catch a glimpse of Zeus or get to challenge Arachnida with your talents. You should however be warned, she has the ability to turn people into spiders!</p>
      </div>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Greece</title>
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" ></style>
<style>
    #map{
        height: 100vh;
        width: 100%;
    }
</style>
</head>
<body>
    <div id="map"></div>
</body>
</html>
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script> 
<script>
    var map = L.map('map').setView([37.983810, 23.727539], 6);

var osm = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
});
osm.addTo(map);

var athens = L.marker([37.98864382281075, 23.73043860232225]);
athens.addTo(map);
var popupAthens =athens.bindPopup('<b> <u> Athens </b> </u> <br> Athens is the capital of Greece. It was also at the heart of Ancient Greece, a powerful civilization and empire. The city is still dominated by 5th-century BC landmarks, including the Acropolis, a hilltop citadel topped with ancient buildings like the colonnaded Parthenon temple.' 
);
popupAthens.addTo(map);
var peloponnese = L.marker([37.350471589490695, 22.352736915352427]);
peloponnese.addTo(map);
var popupPeloponnese =peloponnese.bindPopup('<b> <u> Peloponnese </b> </u> <br> The Peloponnese, Peloponnesus, or Morea is a peninsula and geographic region in southern Greece. It is connected to the central part of the country by the Isthmus of Corinth land bridge which separates the Gulf of Corinth from the Saronic Gulf.')
popupPeloponnese.addTo(map);
var crete = L.marker([35.26804365799052, 24.812047927658206]);
crete.addTo(map);
var popupCrete =crete.bindPopup('<b> <u> Crete Islands </b> </u> <br> Crete is the largest and most populous of the Greek islands, the 88th largest island in the world and the fifth largest island in the Mediterranean Sea, after Sicily, Sardinia, Cyprus, and Corsica. Crete rests about 160 km south of the Greek mainland, and about 100 km southwest of Anatolia')
popupCrete.addTo(map);
var dodecanese = L.marker([36.48068637570861, 26.706662264881462]);
dodecanese.addTo(map);
var popupDodecanese =dodecanese.bindPopup('<b> <u> Dodecanese Islands </b> </u> <br> The Dodecanese, in the southeastern Aegean Sea, is a group of Greek islands known for their medieval castles, Byzantine churches, beaches and ancient archaeological sites. On the largest island, Rhodes, the medieval Street of the Knights and Palace of the Grand Masters show Byzantine and Ottoman influences. Kallithéa and Ialissós are popular beach resorts, and Lindos’ acropolis has panoramic coastal views. ')
popupDodecanese.addTo(map);
var cyclades = L.marker([37.32484743339162, 25.028267458530696]);
cyclades.addTo(map);
var popupCyclades =cyclades.bindPopup('<b> <u> Cyclades </b> </u> <br>The Cyclades is a group of Greek islands, southeast of the mainland in the Aegean Sea. It centers on uninhabited Delos, considered the birthplace of Apollo, and home to some of Greece’s most important archaeological ruins. Many of the islands are popular holiday destinations, known for their beaches, ancient sites, rugged landscapes and traditional blue-and-white stucco towns overlooking the sea. ')
popupCyclades.addTo(map);
var santorini = L.marker([36.41956607246147, 25.427149285549667]);
santorini.addTo(map);
var popupSantorini =santorini.bindPopup('<b> <u> Santorini </b> </u> <br> Santorini is one of the Cyclades islands in the Aegean Sea. It was devastated by a volcanic eruption in the 16th century BC, forever shaping its rugged landscape. The whitewashed, cubiform houses of its 2 principal towns, Fira and Oia, cling to cliffs above an underwater caldera (crater). They overlook the sea, small islands to the west and beaches made up of black, red and white lava pebbles.')
popupSantorini.addTo(map);
var ioannina = L.marker([39.66391786016347, 20.85044745607894]);
ioannina.addTo(map);
var popupIonnina =ioannina.bindPopup('<b> <u> Ionnina </b> </u> <br> Ioannina, often called Yannena within Greece, is the capital and largest city of the Ioannina regional unit and of Epirus, an administrative region in north-western Greece. According to the 2011 census, the city population was 65,574, while the municipality had 112,486 inhabitants.')
popupIonnina.addTo(map);
var mykonos = L.marker([37.44187407583024, 25.368827100117418]);
mykonos.addTo(map);
var popupMykonos =mykonos.bindPopup('<b> <u> Mykonos </b> </u> <br> Mykonos is an island in the Cyclades group in the Aegean Sea. It is popularly known for its summer party atmosphere. Beaches such as Paradise and Super Paradise have bars that blare thumping music. Massive dance clubs attract world-renowned DJs and typically stay open well past dawn. Iconic landmarks include a row of 16th-century windmills, which sit on a hill above Mykonos town.')
popupMykonos.addTo(map);
</script>
