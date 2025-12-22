ERROR - 2025-12-22 13:23:56 --> Query error: [Microsoft][ODBC Driver 11 for SQL Server][SQL Server]Invalid column name 'INV_ASSIGN_NO'. - Invalid query: SELECT TOP 1
                    inv.INV_ID,
                    inv.INV_TOOL_ID AS TOOL_ID,
                    inv.INV_MLR_ID,
                    ml.ML_TOOL_DRAW_NO AS TOOL_DRAWING_NO,
                    mlr.MLR_REV AS REVISION,
                    tc.TC_NAME AS TOOL_NAME,
                    tc.TC_ID AS TOOL_NAME_ID,
                    mat.MAT_NAME AS MATERIAL,
                    mat.MAT_ID AS MATERIAL_ID,
                    ISNULL(ord.ORD_RQ_NO, inv.INV_RQ_NO) AS RQ_NO,
                    mlr.MLR_PRICE AS TOOL_PRICE,
                    inv.INV_ASSIGN_NO AS TOOL_ASSIGNMENT_NO,
                    ISNULL(pcs_produced.PCS_PRODUCED, 0) AS PCS_PRODUCED,
                    inv.INV_STATUS AS STATUS,
                    ISNULL(inv.INV_END_CYCLE, 0) AS END_CYCLE
                FROM TMS_NEW.dbo.TMS_TOOL_INVENTORY inv
                INNER JOIN TMS_NEW.dbo.TMS_TOOL_MASTER_LIST_REV mlr ON mlr.MLR_ID = inv.INV_MLR_ID
                INNER JOIN TMS_NEW.dbo.TMS_TOOL_MASTER_LIST ml ON ml.ML_ID = mlr.MLR_ML_ID
                LEFT JOIN TMS_NEW.dbo.MS_TOOL_CLASS tc ON tc.TC_ID = mlr.MLR_TC_ID
                LEFT JOIN TMS_NEW.dbo.MS_MATERIAL mat ON mat.MAT_ID = inv.INV_MAT_ID
                LEFT JOIN TMS_NEW.dbo.TMS_ORDERING_ITEMS ordi ON ordi.ORDI_ID = inv.INV_ORDI_ID
                LEFT JOIN TMS_NEW.dbo.TMS_ORDERING ord ON ord.ORD_ID = ordi.ORDI_ORD_ID
                LEFT JOIN (
                    SELECT ASSGN_INV_ID, SUM(ISNULL(ASSGN_QTY_PRODUCED, 0)) AS PCS_PRODUCED
                    FROM TMS_NEW.dbo.TMS_ASSIGNED_TOOLS
                    WHERE ASSGN_INV_ID IS NOT NULL
                    GROUP BY ASSGN_INV_ID
                ) pcs_produced ON pcs_produced.ASSGN_INV_ID = inv.INV_ID
                WHERE inv.INV_TOOL_ID = '40010-S0025-HF5'
                ORDER BY inv.INV_ID DESC
