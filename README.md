tambahkn informasi dibawahnya yg isinya
Shared Tool	
ID	Product	Tool BOM
koneksinya yg sama dari product untuk menampilkan tool bom. data diambil dari FROM [TMS_DB].[dbo].[TMS_TC_TOOL_BOM_ENGIN] yg isinya [ID]
      ,[TOOL_BOM]
      ,[PRODUCT]


  SELECT TOP (1000) [STORAGE_LOCATION_ID]
      ,[STORAGE_LOCATION_NAME]
      ,[STORAGE_LOCATION_DESC]
      ,[IS_DELETED]
      ,[DELETED_AT]
      ,[DELETED_BY]
  FROM [TMS_DB].[dbo].[TMS_STORAGE_LOCATION]


SELECT TOP (1000) [REASON_ID]
      ,[REASON_NAME]
      ,[REASON_CODE]
      ,[IS_DELETED]
      ,[DELETED_AT]
      ,[DELETED_BY]
  FROM [TMS_DB].[dbo].[TMS_M_REASON]


SELECT TOP (1000) [CON_ID]
      ,[CON_CURRENCY]
      ,[CON_RATE]
      ,[IS_DELETED]
      ,[DELETED_AT]
      ,[DELETED_BY]
  FROM [TMS_DB].[dbo].[TMS_M_CONVERSION_RATE]
