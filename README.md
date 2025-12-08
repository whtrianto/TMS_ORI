buatkan fie baru khusus untuk edit data bom ini yg berisikan:
Product	:		
DT DCM 10A
 Submit 
Tool BOM	:		
DT DCM 10A
 
Revision	:		
0
 
Process	:		
DIE TRIMMING
 Submit 
Machine Group	:		
DCM CYLINDER
 Submit 
Description	:	 	
015
Status	:	 	
Pending
Effective Date	:		
24-07-2023
 Submit
Change Summary	:	 	
	Additional Information
Drawing	:	

tambahkan juga dibawahnya Additional Information	yg berisi crud
 	No.	ID	Drawing	Tool Drawing No.	Tool Name	Revision	Status	Quantity	Std. Quantity	Sequence	Remarks

  ambil datanya di database SELECT TOP (1000) [TD_ID]
      ,[TD_PRODUCT_ID]
      ,[TD_PROCESS_ID]
      ,[TD_DRAWING_NO]
      ,[TD_TOOL_NAME]
      ,[TD_REVISION]
      ,[TD_STATUS]
      ,[TD_EFFECTIVE_DATE]
      ,[TD_MODIFIED_DATE]
      ,[TD_MODIFIED_BY]
      ,[TD_MATERIAL_ID]
      ,[TD_MAKER_ID]
      ,[TD_MIN_QTY]
      ,[TD_REPLENISH_QTY]
      ,[TD_PRICE]
      ,[TD_TOOL_LIFE]
      ,[TD_DESCRIPTION]
  FROM [TMS_DB].[dbo].[TMS_TC_TOOL_DRAWING_ENGIN]
jika tidak ada colomnya maka buatkan sqlnya untuk tambah colom baru
