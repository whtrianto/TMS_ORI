Screenshot+%282%29.png:1   GET http://localhost/taci-mfg-trial/application/tms_modules/Attachment_TMS/Drawing/73443/0/Screenshot+%282%29.png 403 (Forbidden)
Image
(anonymous) @ jquery.min.js:2
_ @ jquery.min.js:2
html @ jquery.min.js:2
renderFileFromUrl @ index:959
(anonymous) @ index:970
c @ jquery.min.js:2
fireWith @ jquery.min.js:2
l @ jquery.min.js:2
(anonymous) @ jquery.min.js:2
XMLHttpRequest.send
send @ jquery.min.js:2
ajax @ jquery.min.js:2
(anonymous) @ index:898
dispatch @ jquery.min.js:2
v.handle @ jquery.min.js:2
main.js:81 Error message: Uncaught TypeError: Cannot read properties of null (reading 'style')
URL: http://localhost/taci-mfg-trial/tool_engineering/tool_draw_engin/index
Line Number: 1
index:1  Uncaught TypeError: Cannot read properties of null (reading 'style')
    at HTMLImageElement.onerror (index:1:52)



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
