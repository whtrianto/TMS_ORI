buat tampilannya sama dengan 
tapi yg isinya 	ID,	Tool BOM,	Description,	Product,	Machine Group,	Revision,	Status,	Modified By, Action (edit,history,delate)
 	



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
