USING OGR2OSM FOR UVM-SAL BUILDING FOOTPRINTS

- Convert raster to vector, then extract building polygons (usually GRIDCODE = 5)

- Open shapefile in QGIS, import OSM data for the area, select by location for intersection with existing polygon and line features, then switch selection and export "buildings for import" shapefile

- From /Dropbox/Consulting/city_basemaps/osmscripts/ogr2osm/, run 

> ./ogr2osm.py [buildingsforimport].shp

- Open [buildingsforimport].osm in JOSM, run "Search" for "type:way" to select all new buildings

- "Add" Key = Building, Type = yes

- Ship to OSM lists as .osm format to get a doublecheck.

- Upload!
