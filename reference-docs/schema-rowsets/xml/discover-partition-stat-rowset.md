---
title: "DISCOVER_PARTITION_STAT Rowset | Microsoft Docs"
ms.date: 07/25/2018
ms.prod: sql
ms.technology: analysis-services
ms.custom: schema-rowsets
ms.topic: reference
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
---
# DISCOVER_PARTITION_STAT Rowset

  Returns statistics on aggregations in a particular partition.  
  
 **Applies to:** tabular models, multidimensional models  
  
## Rowset Columns  
 The **DISCOVER_PARTITION_STAT** rowset contains the following columns.  
  
|Column name|Type indicator|Restriction|Description|  
|-----------------|--------------------|-----------------|-----------------|  
|**DATABASE_NAME**|**DBTYPE_WSTR**|Required|The name of the database that contains the dimension.<br /><br /> This column is required in the restriction list.|  
|**CUBE_NAME**|**DBTYPE_WSTR**|Required|The name of the cube or tabular model that contains the partition.<br /><br /> This column is required in the restriction list.|  
|**MEASURE_GROUP_NAME**|**DBTYPE_WSTR**|Required|The name of a measure group in the dimension.<br /><br /> This column is required in the restriction list.|  
|**PARTITION_NAME**|**DBTYPE_WSTR**|Required|The name of a partition.<br /><br /> This column is required in the restriction list.|  
|**AGGREGATION_NAME**|**DBTYPE_WSTR**||The name of the aggregation.|  
|**AGGREGATION_SIZE**|**DBTYPE_I8**||The size of the aggregation.|  
  
 This schema rowset is not sorted.  
  
## Using ADOMD.NET to return the rowset  
 When using ADOMD.NET and the schema rowset to retrieve metadata, you can use either the GUID or string to reference a schema rowset object in the GetSchemaDataSet method.
  
 The following table provides the GUID and string values that identify this rowset.  
  
|Argument|Value|  
|--------------|-----------|  
|GUID|a07ccd8f-8148-11d0-87bb-00c04fc33942|  
|ADOMDNAME|PartitionStat|  

