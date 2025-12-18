A PHP Error was encountered
Severity: Notice

Message: Undefined variable: bom

Filename: views/edit_tool_bom_engin.php

Line Number: 30

Backtrace:

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\views\edit_tool_bom_engin.php
Line: 30
Function: _error_handler

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 363
Function: include

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 304
Function: _ci_load

File: C:\laragon_new\www\taci-mfg-trial\application\core\MY_Controller.php
Line: 104
Function: view

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\controllers\Tool_bom_engin.php
Line: 158
Function: view

File: C:\laragon_new\www\taci-mfg-trial\index.php
Line: 329
Function: require_once

A PHP Error was encountered
Severity: Notice

Message: Undefined variable: bom

Filename: views/edit_tool_bom_engin.php

Line Number: 41

Backtrace:

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\views\edit_tool_bom_engin.php
Line: 41
Function: _error_handler

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 363
Function: include

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 304
Function: _ci_load

File: C:\laragon_new\www\taci-mfg-trial\application\core\MY_Controller.php
Line: 104
Function: view

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\controllers\Tool_bom_engin.php
Line: 158
Function: view

File: C:\laragon_new\www\taci-mfg-trial\index.php
Line: 329
Function: require_once

">
Trial BOM

Product
-- Select Product --
Tool BOM
<div style=
A PHP Error was encountered
Severity: Notice

Message: Undefined variable: bom

Filename: views/edit_tool_bom_engin.php

Line Number: 79

Backtrace:

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\views\edit_tool_bom_engin.php
Line: 79
Function: _error_handler

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 363
Function: include

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 304
Function: _ci_load

File: C:\laragon_new\www\taci-mfg-trial\application\core\MY_Controller.php
Line: 104
Function: view

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\controllers\Tool_bom_engin.php
Line: 158
Function: view

File: C:\laragon_new\www\taci-mfg-trial\index.php
Line: 329
Function: require_once

">
Revision
0
Process
-- Select Process --
Machine Group
-- Select Machine Group --
Description
Status
Active
Effective Date
dd/mm/yyyy
Change Summary
Additional Information
DrawingNo file chosen
Biarkan kosong jika tidak mengganti file.
Additional Information (Tool Drawing Engin)
A PHP Error was encountered
Severity: Notice

Message: Undefined variable: additional_info

Filename: views/edit_tool_bom_engin.php

Line Number: 193

Backtrace:

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\views\edit_tool_bom_engin.php
Line: 193
Function: _error_handler

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 363
Function: include

File: C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Loader.php
Line: 304
Function: _ci_load

File: C:\laragon_new\www\taci-mfg-trial\application\core\MY_Controller.php
Line: 104
Function: view

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\controllers\Tool_bom_engin.php
Line: 158
Function: view

File: C:\laragon_new\www\taci-mfg-trial\index.php
Line: 329
Function: require_once
 	



saya ingin ubah untuk data user ngambil di sini 
$db['default'] = array(
	'dsn'	=> 'sqlsrv:server=172.31.42.190,1433;Database=ESIGN',
	'hostname' => '172.31.42.190',
	'username' => 'pkl',
	'password' => 'Taci1234',
	'database' => 'ESIGN',
	'dbdriver' => 'pdo',
	'dbprefix' => '',
	'pconnect' => FALSE,
	'db_debug' => (ENVIRONMENT !== 'production'),
	'cache_on' => FALSE,
	'cachedir' => '',
	'char_set' => 'utf8',
	'dbcollat' => 'utf8_general_ci',
	'swap_pre' => '',
	'encrypt' => FALSE,
	'compress' => FALSE,
	'stricton' => FALSE,
	'failover' => array(),
	'save_queries' => TRUE
);

isi tabelnya 
