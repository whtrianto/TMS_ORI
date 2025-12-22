ERROR - 2025-12-22 13:06:50 --> Query error: [Microsoft][ODBC Driver 11 for SQL Server][SQL Server]Invalid column name 'MAC_DESC'. - Invalid query: SELECT 
                    MAC_ID AS ID,
                    MAC_NAME AS NAME,
                    ISNULL(MAC_DESC, '') AS DESCRIPTION
                FROM TMS_NEW.dbo.MS_MACHINES
                ORDER BY MAC_NAME ASC
