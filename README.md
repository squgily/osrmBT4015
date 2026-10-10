## Essentials to run SIMULATION ONLY (phase 5)

* I have uploaded the buildings_layer and singapore_only.osm.pbf (for impedance matrix) into dropbox, extracted from OSM data: https://www.dropbox.com/scl/fo/j3ewkx96wm1i906tgw31e/AE-ousI2_3UfMBT9BQiHrVw?rlkey=4w9dnxbidvczeyqjbcwpy1qko&st=w5bvl6xd&dl=0
* Generated files from each step have otherwise been uploaded to the repository and the program can be run as normal.


## To run FULL PIPELINE (Data processing included)

OSM street data (open-source):
https://download.geofabrik.de/asia/malaysia-singapore-brunei.html

The following layers were extracted from this source:
* Train, bus and ferry stops
* Health facility POIs
* OSM routing maps 

You can get data_large/building_layer_cleaned.geojson through building_layer_cleaner.py.

I have uploaded as many of my source files as I can to the repo. However, due to github restrictions on file size, some files will have to be downloaded manually: 

Large data downloads:

SLA Cadastral Land Parcel: https://data.gov.sg/datasets/d_e7395d743076a2bcc487b0d12b9bf33b/view

Government housing: https://data.gov.sg/datasets/d_16b157c52ed637edd6ba1232e026258d/view
: all government housing apartment blocks in Singapore.


Building points with year_completed: https://data.gov.sg/collections/22/view
Georeferenced from the csv to get geojson points, then buildingtype/landuse is standardised to follow OSM's labelling

Cell capacity extracted from Singapore's 2025 Master Plan:
https://data.gov.sg/datasets/d_a8c3546b26712e35021f3a681d0353ae/view

All others were extracted and processed from the OneMap API (separate repo).
