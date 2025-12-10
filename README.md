buat 
ID,	Tool Tag,	Product,	Tool Name,	Tool Drawing No.,		Tool ID,	Status(New,Allocated,Available,In Used,Onhold,Scrapped,Reprairing,Modifying,Design Change),      Notes,	End Cycle,      Action(edit,delete)

gagal hapus data di 
ERROR - 2025-12-10 13:58:36 --> Query error: [Microsoft][ODBC Driver 11 for SQL Server][SQL Server]The DELETE statement conflicted with the REFERENCE constraint "FK_HISTORY_MAIN_TD". The conflict occurred in database "TMS_DB", table "dbo.TMS_TC_TOOL_DRAWING_ENGIN_HISTORY", column 'TD_ID'. - Invalid query: DELETE FROM "TMS_DB"."dbo"."TMS_TC_TOOL_DRAWING_ENGIN"
WHERE "TD_ID" = 26
