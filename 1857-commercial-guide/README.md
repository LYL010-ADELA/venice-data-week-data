# 1857 Commercial Guide: Data description

The main file for this dataset is called `1857_commercial_guide_with_pages_{date of production}.csv`. It corresponds to the transcription, standardisation and semantic parse of part of the data that can be found in the digitzed commercial guide which is available here in the PDF `1857_Nuova_Guida_commerciale_della_citta_di_Venezia.pdf`. Each entry of the CSV file correspond to a single entry in the commercial guide.

* `LAST_N`: Last name of the person exercising a professional activity.
* `FIRST_N`: First name of the person exercising a professional activity
* `PER_GRP`: Information relating to relationship between the different workers in an entry, for instance if they are siblings ("fratelli" or "sorelle").
* `PER_COMPL`: Complementary information relating to the person, often contains the filiation.
* `LOC_PAR`: Location of the parish where the person is exercising their profession.
* `LOC_STR`: More precise location where the person is exercising their profession, likely the name of the street.
* `NUM`: House number where the person is exercising their profession.
* `LOC_COMPL`: complementary information regarding the location where the person is exercising their profession.
* `DISTRICT`: Venetian district where the person is exercising their profession.
* `geometry`: GPS coordinates in CSR WGS:84 of where we geolocated the worker's place.
* `geometry_from`: The aforementionned geolocation has been provided using different methods, this fields references which method was used to produce the current coordintes: `contemporay` means the contemporary location of house number was used. `cadaster` means the house number as located in different XIXth century-era landregisters. `manuel` means the location was done manually. `interpolation` means that the house number was geolocated by interpolating linearly its position relative to the two closest geolocated point in the sequence of house numbers. 
* `profession`: The profession exerced by the person.
* `profession_en`: translation in english of the aforementioned field.
* `category`: macro categorisation of the profession.
* `category_en`: translation in english of the aforementioned field.
* `PAGE_NUM`: the page index where the current entry appeared in the original digitized document. This relates to the document page, that can be read on top of each scan, and not the page indices of the PDF. To find the page in pdf from this field, add 7 to it.
