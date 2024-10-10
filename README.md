# Ahmet Rende | Database Scripts

## Açıklama
This repository contains various scripts for database systems.

## Contents
- [sp_ManageReadOnlyRouting.sql](./sp_ManageAGReadOnlyRouting/sp_ManageAGReadOnlyRouting.sql): Managing read-only routing for Microsoft SQL Server Availability Groups.

## Example Usage

```sql
EXEC dbo.sp_ManageAGReadOnlyRouting 
	    @DatabaseName	= 'DBNAME'
	   ,@ThresholdSec	= 60
	   ,@HistoryTableFQDN	= 'DBA.dbo.ag_read_only_routing_history'
