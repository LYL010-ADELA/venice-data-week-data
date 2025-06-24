# 946 - 1408 Tables


# Files

- `*.xlsx`: The file name contains the scanned page number and the column number (same as *.json in the `matches` folder).

# Data Fields

## *.xlsx

- `page`: original page number from the book
- `parcel_numbers`: zone number(s) of the quarter
- `map_number`: scanned page number of the geometry
- `informazioni urbinistico-edilizie`: place information in Latin
- `proprietà`: ownership information in Italian
- `sources`: source(s) of the observation
- `dates_start`: start date of the observation date
- `dates_end`: end date of the observation date (differs from the start date if the date is an interval)

`map_number` and `parcel_numbers` can be used to link the ownership and place information to the geometries in the `geometries` folder.