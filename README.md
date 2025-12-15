ERROR - 2025-12-15 11:07:31 --> Severity: Notice --> Undefined property: CI::$db_tms C:\laragon_new\www\taci-mfg-trial\application\third_party\MX\Controller.php 59
ERROR - 2025-12-15 11:07:31 --> Severity: Error --> Call to a member function query() on null C:\laragon_new\www\taci-mfg-trial\application\tms_modules\Tool_engineering\controllers\Tool_draw_engin.php 690




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
