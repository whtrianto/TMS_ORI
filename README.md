
ERROR - 2025-12-08 14:05:19 --> Query error: [Microsoft][ODBC Driver 11 for SQL Server][SQL Server]The INSERT statement conflicted with the CHECK constraint "CK_TMS_TC_TOOL_BOM_ENGIN_Status". The conflict occurred in database "TMS_DB", table "dbo.TMS_TC_TOOL_BOM_ENGIN", column 'STATUS'. - Invalid query: INSERT INTO "TMS_DB"."dbo"."TMS_TC_TOOL_BOM_ENGIN" ("TOOL_BOM", "DESCRIPTION", "REVISION", "STATUS", "PRODUCT_ID", "PROCESS_ID", "MACHINE_GROUP_ID", "PRODUCT", "MACHINE_GROUP", "EFFECTIVE_DATE", "CHANGE_SUMMARY", "DRAWING", "MODIFIED_BY") VALUES ('jg', 'ccc', 0, 1, 3, 13, 1, 'DT DCM 10A', 'TESSS', '2025-12-08 00:00:00', 'jb', 'BOM_1765177518_36300-E4160__2_.jpg', '3333333')

SELECT name, definition
FROM sys.check_constraints
WHERE parent_object_id = OBJECT_ID('TMS_DB.dbo.TMS_TC_TOOL_BOM_ENGIN');
