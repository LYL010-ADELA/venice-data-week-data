# 946 - 1408 Dorigo Entities

This folder contains potential matches of place names, spatial features, person names, family relations, and ownership types against several lists of entries (see `indices` folder and `additional_lists.txt` file).

# Files

- `*.json`: The file name contains the scanned page number and the column number.
- `additional_lists.txt`: English correspondences to Latin and Italian words
- `files.json`: list of file names (only needed for the Data Viewer)
- `index.html`: code for the Data Viewer

# Data Fields

## *.json

- `page_nr`: original page number from the book
- `area_code`: zone number(s) of the quarter
- `map_number`: scanned page number of the geometry
- `date_start`: start date of the observation date
- `date_end`: end date of the observation date (differs from the start date if the date is an interval)
- `source`: source(s) of the data
- `spatial_information`: place information in Latin
- `ownership`: ownership information in Italian
- `matches`: categories and words matched from the `additional_lists.txt` file and an index listing person and place names

`map_number` and `area_code` can be used to link the ownership and place information to the geometries in the `geometries` folder.
Please find a clean version of the area code in the `tables` folder.

## Simple Data Viewer

Serve the files with a simple HTTP server from this directory to view them in a browser, e.g.
```
"C:\Python310\python.exe" -m http.server
```
Open the browser and navigate to `http://localhost:8000/` to view `index.html`.
The matched entities are underlined with different colors.