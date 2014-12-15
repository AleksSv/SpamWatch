SpamWatch
=========

Demo: http://104.236.46.207/~aleks/spamWatch/maps.html

Geolocational Display of unwanted access attempts from foreign IPs

The purpose of this exploration is to display the geolocational data derived from Whois lookups in a more visually appealing way. For this I will use Google Maps API

Google Maps
=============
https://developers.google.com/maps/documentation/javascript/tutorial

The API requires a Google specific API key, which can be registered in the developers section of Google.

The Maps API works in an object orientated way, to set up the demo I used a few of the many features of the API.

Markers
========
https://developers.google.com/maps/documentation/javascript/markers

https://developers.google.com/maps/documentation/javascript/examples/marker-simple

Markers can be connectioned to a location on the map with a set of coordinates, from the JSON data I could acquire the coordinates necessary. With these coordinates all the markers were instantiated on the map with the initMarkersArray() method.

InfoWindows
========
https://developers.google.com/maps/documentation/javascript/infowindows

Are information toolboxes that occur when a click event is registered with a marker, using the other information from the JSON data, I could display other facters relating to each marker, such as number of attempts and regional information.

I had trouble with the same InfoWindow being displayed for each marker and went to stack overflow for solutions

http://stackoverflow.com/questions/5736691/google-maps-infowindow-showing-on-wrong-marker

Turns out that using a seperate function for each marker creation is necessary for data staying consistent
