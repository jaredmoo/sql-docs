---
title: "Global Settings (Logging)  (MySQLToSQL) | Microsoft Docs"
ms.prod: "sql-non-specified"
ms.custom: ""
ms.date: "01/19/2017"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "sql-ssma"
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Azure SQL Database"
  - "SQL Server"
ms.assetid: 0d033492-5ec3-473a-8de1-821894ec9518
caps.latest.revision: 4
author: "sabotta"
ms.author: "carlasab"
manager: "lonnyb"
---
# Global Settings (Logging)  (MySQLToSQL)
Use the **Global Settings** dialog box to specify the logging settings for SSMA. Typically, you would change these settings only when working with product support.  
  
To access this dialog box, on the **Tools** menu, select **Global Settings** and then click the **Logging** button at the bottom of the left pane.  
  
## Options  
**Messages Level**  
The following options are available under **Messages Level**:  
  
|Option|Description|  
|----------|---------------|  
|**[all categories]**|Used to set the logging level for all of the following options.|  
|**Collector**|Collects metadata about the source schema and saves it to the project.|  
|**Converter**|Converts structures of source database objects, such as tables and stored procedures, into corresponding [!INCLUDE[ssNoVersion](../../includes/ssnoversion_md.md)] structures.|  
|**Data migrator**|Migrates data from the source database into [!INCLUDE[ssNoVersion](../../includes/ssnoversion_md.md)].|  
|**Formatter**|Sub-component of the Converter that generates scripts for the [!INCLUDE[ssNoVersion](../../includes/ssnoversion_md.md)] schema.|  
|**Graphical user interface**|Messages that appear when you use the SSMA tool.|  
|**Linker**|Resolves SQL identifiers and provides information to other components.|  
|**Other**|All messages that are not in any other category.|  
|**Parser**|Parses the source schema.|  
|**Synchronizer**|Loads source database objects into [!INCLUDE[ssNoVersion](../../includes/ssnoversion_md.md)].|  
|**TreeConverter**|Converts objects in the source metadata into [!INCLUDE[ssNoVersion](../../includes/ssnoversion_md.md)] metadata.|  
  
For each option under **Messages Level**, configure one of the following logging levels for SSMA:  
  
|||  
|-|-|  
|**Fatal Error**|Write only fatal error messages to the log.|  
|**Error**|Write error and fatal error messages to the log.|  
|**Warning**|Write warning, error, and fatal error messages to the log.|  
|**Info**|Write informational, warning, error, and fatal error messages to the log.|  
|**Debug**|Write all messages, including debugging messages, to the log.|  
  
**Log File path**  
The file path and name of the SSMA log files. To specify a different name, click the current path, and then click the Browse (**...**) button.  
  
**Log File size**  
The maximum size of the log file in KB. The minimum size is 10 KB. The default size is 10240 KB.  
  
**Total number of log files**  
When one log fills, SSMA will rename the log file and start a new one. By using this setting, specify the maximum number of log files to keep. The minimum is 2.  
  