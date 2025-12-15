nomor 1 isi tabelnya
MLR_DRAWING	varchar	50	YES
MLR_SKETCH	varchar	50	YES

nomor 2
kosong/gak ada apa-apa

nomor 3
73443	Screenshot (2).png	NULL	18	NULL	Contains special chars (might be encoded)	NULL
73441	36300-E4160.jpg	NULL	15	NULL	Contains special chars (might be encoded)	NULL
73440	16500-E8790-A_SKE.pdf	NULL	21	NULL	Contains special chars (might be encoded)	NULL
73438	16500-E8790-A_SKE.pdf	NULL	21	NULL	Contains special chars (might be encoded)	NULL
73437	311-073-011 (011A & 011B).jpg	NULL	29	NULL	Contains special chars (might be encoded)	NULL

nomor 4
sysdiagrams	definition	varbinary	-1

nomor 5
sysdiagrams	definition	varbinary	-1




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
