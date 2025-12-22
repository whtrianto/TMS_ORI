A Database Error Occurred
Error Number: 42000/156

[Microsoft][ODBC Driver 11 for SQL Server][SQL Server]Incorrect syntax near the keyword 'USER'.

SELECT USR_ID AS ID, USR_NAME AS USER, ISNULL(USR_POSITION, '') AS POSITION FROM TMS_NEW.dbo.MS_USERS WHERE USR_IS_DELETED = 0 OR USR_IS_DELETED IS NULL ORDER BY USR_NAME ASC

Filename: C:/laragon_new/www/taci-mfg-trial/system/database/DB_driver.php

Line Number: 691
