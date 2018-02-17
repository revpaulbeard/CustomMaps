CustomMaps
A combination of tools to make custom Google Maps

A FORMATTED COPY OF THIS FILE IS IN CustomMaps.docx

mapfromjsxml.html
This HTML/JavaScript application takes data from a file "Map.js" which is a simple declaration of an XML file as a JavaScript string. The data contains address or lat/lng coordinates for position and draws markers on a map in all major browsers using GoogleMaps API v3. 
A sidebar lists the entries corresponding to groups and markers. (Where no position information can be located, there is no corresponding marker.)
Each marker is (optionally) numbered and (automatically) has an infoWindow associated with it which opens on clicking the marker or corresponding sidebar entry.
	The markers use custom shapes (based on SVG descriptions.) The shape, font colour and fill colour are determined by group headers to which the marker data refers.
	Where lat/lng coordinates are missing the application will GeoCode the address.
	Markers can be moved and the new lat/lng coordinates are displayed.
Polygons can also be added to the map.
	Various display options and reports are available.
Notes:	In the UK, GeoCoding is to postcode level (courtesy of Royal Mail.)
A fixed file named "Map.js" – which must reside in the same directory – contains the data to be included in the application.
The application uses the file "markerwithlabel.js" (author Gary Little (inspired by code from Marc Ridey of Google). © 2012 Gary Little [gary@luxcentral.com])

XML joinup.docm
This is a macro-enabled document used to convert an XML file into its JavaScript counterpart for use with mapfromjsxml.html. 
The VBA macro takes information from files in the same directory named "MapXMLHeader.xml" and "Map.xml" to create the file "Map.js"
MS Excel
A macro-enabled MS Excel spreadsheet may be used to prepare the data for the XML file in a user-friendly way. An example is contained in the file "MapXMLExample.xlsm"
" MapEntries.xsd" is a schema file for the spreadsheet to use in attaching data to XML tags. " Map.xsd" contains the schema including the header. 
Note: Group headers are distinguished by having a negative value in "sbindex".
In the example the raw data is held in Sheet ""DB Processing". The "Scratch" sheet is used to consolidate and prepare the data. From there it can be pasted (Paste Special – Values & Formats) into the "XML ready" Sheet. 
This example does not fully reflect what is available in the mapfromjsxml.html  application.


