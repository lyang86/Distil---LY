// Root URL to get Train Arrival Times
$apiURL = "http://api.wmata.com/StationPrediction.svc/json/GetPrediction/";

//Station Code; currently set for Ballston.
$stationCode = "K04";
headers = {Next arrival of Orange line train from current time

// API Key for WMATA
$apiKey = "kfgpmgvfgacx98de9q3xazww";

//Rail line code you are looking for; currently set for Orange line.
$lineCode = "OR";
 
//('https://api.wmata.com/StationPrediction.svc/json/GetPrediction/{Ballston}')
 
//uri.query = URI.encode_www_form({
    # Specify your subscription key
    'api_key' => 'kfgpmgvfgacx98de9q3xazww',
})
 
//# Basic Authorization
# request.basic_auth 'lyang86', 'New1Pass'
 
 //Check if arriving train is Orange Line
if($train["Line"]==OR){
$destName = $train["BALLSTON"];
$dest = $train["K04"];
$min = $train["Min"];

if($min=="ARR"){ //Custom message if train is currently arriving
$message = "The Orange Line train is ARRIVING NOW at Ballston"
