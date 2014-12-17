db-to-api-package
=================

Composer package for converting database to api (github.com/project-open-data/db-to-api)

USAGE
-------------
intialize the api variable in routes/controller as

$var = Eddywebs\DbToApi\DbToApi::getApi($param, $config);


Where $param has the parameters for returning data, params little different from the paramater url in the readme file of original code at github.com/project-open-data/db-to-api.

$config is array of configuration in following format:
$config = array( 
             'name' => 'database-name',
             'username' => 'username',
             'password' => 'password',
             'server' => 'hostname',
             'port' => port-number,
             'type' => 'supported-database-type', 
             'table_blacklist' => array(),
             'column_blacklist' => array(),
 );

Databases Supported
-------------------

* 4D
* CUBRID
* Firebird/Interbase
* IBM
* Informix
* MS SQL Server
* MySQL
* ODBC and DB2
* Oracle
* PostgreSQL
* SQLite

Param/url structure
-------------------
* All rows in table: db=dataset-name&table=datasets&format=json
* A specific row in a table: db=dataset-name&table=datasets&value=ID&format=json


