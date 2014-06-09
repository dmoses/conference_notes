## GIS Workshop - June 9 - Morning

### Fieldtrip GB

* [http://fieldtripgb.blogs.edina.ac.uk/](http://) 
* works without GPS
* doesn't rely on grid
* potentially something to look at for fieldwork ... recording specimen data, etc.

### Hands-on using qgis and data sets.

* see handout
* created map using raster (image), vector(points), and wms(map base) layers ... historical buildings in Edinburgh.
* QGIS Plugins
     * OGR ... create a exported version of the work you did to put on the web as an interactive map.

### GIS in Digital Repositories

* [slides](https://docs.google.com/a/upei.ca/file/d/0B5fLh2mc4FCbMFFPQjJtX1hidW8/edit)
* metadata and wrangling > curation > delivery > discovery
* Hydra ... community and tech framework ... repo with many diff heads
	* hydra head (CRUD), Blacklight (Read), Fedora, Solr (Solrizer) ... could we use solrizer in Islandora and get rid of GSearch?
* vector data - point, line, polygon - GeoBlackLight
* historic maps can be georectified ... transparency allows you to view basemap
* raster data - modelled output ..eg population data, can also be imagery ... 
* GIS Data
	* layers of data (eg. vector and rastor)
	* those and other assets with geo properties ... eg. a postcard with coordinate data
* Discovery
	* see slide 20 for screencast link, etc.
	* see discovery use cases in slides 22 and 23 
	* GeoBlacklight demo ... really nice
	* MODS metadata ... extension element with custom schema to record bounding box data ... maybe ESRI?
	* Geoportal
		* http://geodata.tufts.edu - is another way to  discover GIS data
	* BlackLight Maps
		* tool to map results that have coordinate info
		* clustering 
		* alternative views
		* eg. scanned maps that have a bounding box ... but have not been georectified
	* Bassi-Veratti Collection
		* custom application for manuscripts with geo data ... eg letters tagged with Florence.
		* spatial view of the content
		
### GeoServer

* important part of GIS infrastructure
* plug in various database servers ... output various servers
* GDAL ... important as well ... conversion utility ... many file formats supported
* GeoTIFF and Shapefiles as canoncial formats at Stanford 


## Workshop PM

* Spent first part of the afternoon learning about web based metadata creation tools. Creating metadata records with GoGeo ... 
http://www.gogeo.ac.uk

### Delivery of GIS data

#### Open GeoSuite
**GeoServer**

* missed this explanation ... 

**Caching Server**

* GeoWebCache - tile server
* GeoServer talks to GeoWebCache

**PostGIS**

* PostgreSQL is underneath
* query-able ... intersections or other types of geo math.

### Repository

**Stanford**
* Digital object model
	* each GIS layer is a digital boejct
	* many GIS layers are a digital collection
	* Datastreams metadata
		* MODS "geo" extension
		* ISO 19139/19110 for GIS datasets
		* Linked data for place names (eg. gazetteer) 
* ARGO used to manage ingest/object streams
* ArcCatalog used for metadata authoring
* metadata 
* start > druid (ID) > author metadata > approve metadata ... then a split >
	* extract tn
	* extract-iso19139 > generate mods > assign-placenames (using GeoNames)> finish metadata
* data
* start > druid (ID) > wrangle data (eg. projection, attribute table, format ... understanding the data... then use GDAL to transform into a canoncial projection that would be put into your spatial data framework) > approved-data > finish data
* generate content-metadata > finish > start assemblyWorkFlow and gisDeliveryWorkflow
* gisDeliveryWF 
	* start > load-vector and load-raster > load-geoserver ... 
* gisDiscoveryWF
	* generate geosearch > load... 
	* generate-ogp > ...
	
MODS metadata extension as RDF
gml:Envelope 
gml:lowerCorner
gml:upperCorner
dc:coverage red:resource="http://sws.geonames.org/1269328/about.rdf" dc:language="eng" dc:...
linked data to GeoNames and lcnaf entries for the places.

Demonstration of ARGO 

* lots of metadata streams ... descmetadata, provmetadata, events, etc.

### Gazetteer Web Services

* aggregator of data sources
	* search, postCodeSearch
	* hierarchy
* integration
	* with GeoNames
	     * rdf, geotree, kml
	     * alternative names
	    	 * to LCNA, to wikipedia article, ... 
	* with LCSH
	* with LibCongress Name Authorities
	* MARC records can be enriched 
* CLAVIN for natural language processing. http://clavin.bericotechnologies.com/
  * dm note: we've used ANNIE/GATE and have been experimenting with OpenCalais

