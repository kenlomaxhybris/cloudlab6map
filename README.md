Set up Google Account 
=====================
Set up Google Account with Map and Geocoding service and get its API key for it:
cloudlab620190321@gmail.com
https://console.cloud.google.com
Create Project cloudlab620190321
https://developers.google.com/maps/documentation/javascript/get-api-key

Run locally on OSX
=====================
python -m SimpleHTTPServer 8080
http://localhost:8080/mymap.html?END_POINT=http://localhost:8017/purchasesByNameSpace?nameSpace=space1

Build docker image
=====================
docker build -t kenlomax/cloudlab620190321:v1 .
docker push kenlomax/cloudlab620190321:v1
(-> https://cloud.docker.com/u/kenlomax/repository/docker/kenlomax/cloudlab620190321)
docker run -d -p 80:80 kenlomax/cloudlab620190321:v1
http://localhost/mymap.html?END_POINT=https://xfcl20190322a.elastic-bose.cluster.extend.sap.cx/purchasesByNameSpace?nameSpace=space1

Run from any docker
=======================
docker run -d -p 8080:80 kenlomax/cloudlab620190321:v1
http://localhost:8080/mymap.html?END_POINT=https://xfcl20190322a.elastic-bose.cluster.extend.sap.cx/orders

