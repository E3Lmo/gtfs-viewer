# GTFS Transit Route Viewer #
*This application is a viewer to display general transit feed specification (GTFS) data in a web browser. Its intent is to act as an auditing tool for GTFS data or to be modified for implementation with a transit agency trip planning system.*

[![GTFS Viewer Screenshot](https://github.com/jonkostyniuk/gtfs-viewer/blob/master/SCREENSHOT.png?raw=true)](https://github.com/jonkostyniuk/gtfs-viewer/blob/master/SCREENSHOT.png?raw=true)

## Versions ##
V0.1a, Build XX, Released 2015-08-XX (COMING SOON)

## Implementation ##
Start a local web server by running the following from the command line:

	python app.py
	
Load the following web page to interact with the program:
	
	http://localhost:8080/ 

## Testing ##
This software is currently considered in ALPHA status, meaning that testing is still ongoing and all functionality has yet to be implemented. **Use at your own risk.**

The current version has primarily been released as proof-of-concept and is not ready for production purposes at this time.

Development and testing to date has primarily been in the *Google Chrome* browser. Unexpected functionality may occur with other browsers at this time.

Open-source GTFS transit data was used in the testing of this application from the following transit agencies:
* [Calgary Transit](http://www.calgarytransit.com)
* [Halifax Transit](http://www.halifax.ca/transit/)
* [Kingston Transit](http://www.kingstontransit.ca)
* [Saskatoon Transit](https://transit.saskatoon.ca/)
* [Winnipeg Transit](http://www.winnipegtransit.com)
* [York Region Transit](http://www.yrt.ca)

## Dependencies ##
The GTFS Viewer is built upon several third-party, open-source dependency packages to provide functionality.

### Python ###
* Flask >=0.10.1
* pandas >=0.16.1
* requests >=2.2.1

### HTML/CSS/JavaScript ###
* JQuery >=1.11.2
* Bootstrap >=3.3.4
* Moment >=2.10.3
* Bootstrap-DateTimePicker >=4.14.30
* Spin >=2.3.1
* Google Maps API >=3.21

## Current Features ##
The GTFS Viewer presently features the following functionality:
* Select GTFS files from preloaded, unzipped dropdown. Folder structure uses './[UUID]/[Timestamp]/' structure to contain unzipped GTFS files.
* Select from routes loaded on-the-fly from GTFS files.
* Specify date/time of trip desired.
* API based on agency, route, and date/time request will fetch route polylines and dynamically display on map using Google Maps API.
* Zoom in to see stop level detail and stop locations.

## Future Development ##
Ongoing development of this repository may include the following potential features:
* Pull GTFS data directly from www.gtfs-data-exchange.com
* Upload functionality for zipped GTFS files.
* Inter-relation with other stops and routes.

## Project Inspiration ##
Why did I create this project? Honestly, similar applications have been created for transit agencies, so this really is nothing new.

This project was created so that I could further develop my skills in the following areas:
* Using the Flask Python framework for API backend development.
* Working with the GTFS protocol for transit planning and routing.
* Gain more experience using the Pandas Python package for data analysis.

## Contact ##
For questions or information about this repository, please contact:

jon.kostyniuk@gmail.com

## License ##
This code is released under the MIT License

https://github.com/jonkostyniuk/gtfs-viewer/blob/master/LICENSE

Copyright (c) 2015 Jon Kostyniuk
