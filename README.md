db-to-api-package
=================

Composer package for converting database to api (github.com/project-open-data/db-to-api)

intialize the api variable in routes/controller as

$var = Eddywebs\DbToApi\DbToApi::getApi($param);

Where $param has the parameters for returning data, params little different from the paramater url in the readme file of original code at github.com/project-open-data/db-to-api.

Param/url structure
-------------------
* All rows in table: db=dataset-name&table=datasets&format=json
* A specific row in a table: db=dataset-name&table=datasets&value=ID&format=json


