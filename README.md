## xspectrolum01-setup_db

Python package for setting up a Postgres database for
xspectrolum spectral library

### Introduction

xspectrolum spectral library is an attempt for semi-automated processing of spectral data.
The database setup (setup_db) package contains the processing for
setting up the xspectrolum spectral library postgreSQL database. The package contains the following (**.py**) modules:


- \_\_init.py\_\_
- param_json_mini.py
- setup\_db\_class.py
- setup\_db\_main.py
- version.py

### Built for Eclipse

The package is part of a larger superproject - xspectrolum. The package is built using Eclipse but can also be run stand alone.

To run the package you must create a json file under your local user on the machine. The jsone file must be under the path ~/xspectrolum/xspectrolum/speclib_default.json:
```
{
  "postgresdb": {
    "db": "speclib"
  },
  "userproject": {
    "userid": "xspectre"
  },
  "process": [
    {
      "verbose": 2,
      "overwrite": false,
      "delete": false,
      "acceptmissing": true,
      "dryrun": false,
      "wgetpath": "/usr/local/bin",
      "inkscapepath": "/Applications/Inkscape.app/Contents/MacOS/inkscape",
      "srcpath": {
        "volume": "~",
        "hdr": "txt"
      },
      "dstpath": {
        "volume": "~",
        "hdr": "txt"
      }
    }
  ]
}
```

### Package complete content

```
.
|____version.py
|______init__.py
|____paramjson_mini.py
|____setup_db_class.py
|____setup_db_main.py
|____README.md
|____LICENSE
|____.gitignore
|____doc
| |____db_speclib_setup_20230108.txt
| |____db_speclib_delete_20220601.txt
| |____db_speclib_dbusers_20220601.txt
| |____jsonsql
| | |____general_spectrascan_v090_sql.json
| | |____general_grant_speclib_v090_sql.json
| | |____general_campaign-meta_v090_sql.json
| | |____general_probeobs_v090_sql.json
| | |____general_schema_v090_sql.json
| | |____.DS_Store
| | |____general_refspectra_main+meta_v090_sql.json
| | |____db-delete_v090.json
| | |____general_lights_v090_sql.json
| | |____general_sensors_v090_sql.json
| | |____general_support_records_v090_sql.json
| | |____general_spectrometer_v090_sql.json
| | |____general_ancillary_v090_sql.json
| | |____general_processes_v090_sql.json
| | |____general_campaign-main_v090_sql.json
| | |____general_processes_records_v090_sql.json
| | |____general_support_v090_sql.json
| |____dbdelete
| | |____drop_sensors_tables.sql
| | |____drop_xspect_tables.sql
```
