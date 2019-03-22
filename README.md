Set up Google Account 
=====================
Set up Google Account with Map and Geocoding service and get its API key for it:
cloudlab620190321@gmail.com
https://console.cloud.google.com
Create Project cloudlab620190321
https://developers.google.com/maps/documentation/javascript/get-api-key


Run locally
=====================
python -m SimpleHTTPServer 8000
http://localhost:8000/mymap.html?END_POINT=https://xfcl20190322a.elastic-bose.cluster.extend.sap.cx/orders


Build docker image
=====================
docker build -t mymaps:v1 .
docker run -d -p 80:80 mymaps:v1
http://localhost/mymap.html?END_POINT=https://xfcl20190322a.elastic-bose.cluster.extend.sap.cx/orders


