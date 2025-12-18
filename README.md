Error Number: 42S22/207

[Microsoft][ODBC Driver 11 for SQL Server][SQL Server]Invalid column name 'ML_IS_TRIAL_BOM'.

SELECT rev.MLR_ID AS TD_ID, rev.MLR_ML_ID, rev.MLR_OP_ID, rev.MLR_MACG_ID, ml.ML_TOOL_DRAW_NO AS TD_TOOL_BOM, ml.ML_IS_TRIAL_BOM, ISNULL(rev.MLR_DESC, '') AS TD_DESCRIPTION, ISNULL(dbo.fnGetToolMasterListParts(ml.ML_ID), '') AS TD_PRODUCT_NAME, ISNULL(mac.MAC_NAME, '') AS TD_MACHINE_GROUP, rev.MLR_REV AS TD_REVISION, rev.MLR_STATUS AS TD_STATUS, ISNULL(usr.USR_NAME, '') AS TD_MODIFIED_BY, CASE WHEN rev.MLR_MODIFIED_DATE IS NULL THEN '' ELSE CONVERT(VARCHAR(19), rev.MLR_MODIFIED_DATE, 120) END AS TD_MODIFIED_DATE, CASE WHEN rev.MLR_EFFECTIVE_DATE IS NULL THEN '' ELSE CONVERT(VARCHAR(19), rev.MLR_EFFECTIVE_DATE, 120) END AS TD_EFFECTIVE_DATE, rev.MLR_CHANGE_SUMMARY AS TD_CHANGE_SUMMARY, ISNULL(rev.MLR_DRAWING, '') AS MLR_DRAWING FROM TMS_NEW.dbo.TMS_TOOL_MASTER_LIST_REV rev INNER JOIN TMS_NEW.dbo.TMS_TOOL_MASTER_LIST ml ON ml.ML_ID = rev.MLR_ML_ID LEFT JOIN TMS_NEW.dbo.MS_MACHINES mac ON mac.MAC_ID = rev.MLR_MACG_ID LEFT JOIN TMS_NEW.dbo.MS_USERS usr ON usr.USR_ID = rev.MLR_MODIFIED_BY WHERE ml.ML_TYPE = 2 AND rev.MLR_ID = 72957

Filename: C:/laragon_new/www/taci-mfg-trial/system/database/DB_driver.php

Line Number: 691



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
