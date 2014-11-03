shp2kml
=======

shp2kml converts shapefile data to KML and writes it to stdout. It expects a field called "FULLNAME" to exist in the shapefile, and uses that field for the name of each KML Placemark. It currently creates a KML Placemark object for each shape in the shapefile data, and adds a LineString to the Placemark for each point in the shape.

You'll need to pip install the following Python packages:
* pyshp
* lxml
* pykml

Usage: python shp2kml.py <shp file> <dbf file>
