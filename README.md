A PHP Error was encountered
Severity: Warning

Message: ini_set(): A session is active. You cannot change the session module's ini settings at this time

Filename: Session/Session.php

Line Number: 314

Backtrace:

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Attachment_TMS\controllers\Attachment_TMS.php
Line: 24
Function: __construct

File: C:\laragon_new\www\taci-mfg-trial\index.php
Line: 329
Function: require_once

A PHP Error was encountered
Severity: Notice

Message: A session had already been started - ignoring session_start()

Filename: Session/Session.php

Line Number: 143

Backtrace:

File: C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Attachment_TMS\controllers\Attachment_TMS.php
Line: 24
Function: __construct

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
