    public function get_tool_inventory_for_modal()
    {
        $sql = "SELECT TOP 500
                    inv.INV_ID AS ID,
                    LTRIM(RTRIM(inv.INV_TOOL_ID)) AS TOOL_ID,
                    ISNULL(ml.ML_TOOL_DRAW_NO, '') AS TOOL_DRAWING_NO,
                    ISNULL(mlr.MLR_REV, 0) AS REVISION,
                    ISNULL(tc.TC_NAME, '') AS TOOL_NAME,
                    CASE inv.INV_STATUS
                        WHEN 1 THEN 'New'
                        WHEN 2 THEN 'Allocated'
                        WHEN 3 THEN 'Available'
                        WHEN 4 THEN 'InUsed'
                        WHEN 5 THEN 'Onhold'
                        WHEN 6 THEN 'Scrapped'
                        WHEN 7 THEN 'Repairing'
                        WHEN 8 THEN 'Modifying'
                        WHEN 9 THEN 'DesignChange'
                        ELSE 'Unknown'
                    END AS TOOL_STATUS,
                    ISNULL(inv.INV_NOTES, '') AS REMARKS
                FROM {$this->t('TMS_TOOL_INVENTORY')} inv
                INNER JOIN {$this->t('TMS_TOOL_MASTER_LIST_REV')} mlr ON mlr.MLR_ID = inv.INV_MLR_ID
                INNER JOIN {$this->t('TMS_TOOL_MASTER_LIST')} ml ON ml.ML_ID = mlr.MLR_ML_ID
                LEFT JOIN {$this->t('MS_TOOL_CLASS')} tc ON tc.TC_ID = mlr.MLR_TC_ID
                WHERE inv.INV_TOOL_ID IS NOT NULL 
                    AND LTRIM(RTRIM(inv.INV_TOOL_ID)) <> ''
                    AND inv.INV_STATUS <> 6
                    AND ml.ML_TYPE = 1
                ORDER BY inv.INV_TOOL_ID ASC";
        $q = $this->db_tms->query($sql);
        return $q && $q->num_rows() > 0 ? $q->result_array() : array();
    }
