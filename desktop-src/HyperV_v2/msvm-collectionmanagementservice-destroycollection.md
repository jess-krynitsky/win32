---
Description: Deletes the given CIM\_CollectionOfMSEs object.
ms.assetid: 2c79e281-44c3-4a91-98d5-fdf973d149c3
title: DestroyCollection method of the Msvm_CollectionManagementService class
ms.topic: reference
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- Msvm_CollectionManagementService.DestroyCollection
api_type: 
- COM
api_location: 
- vmms.exe
---

# DestroyCollection method of the Msvm\_CollectionManagementService class

Deletes the given [**CIM\_CollectionOfMSEs**](cim-collectionofmses.md) object.

## Syntax


```mof
uint32 DestroyCollection(
  [in]  CIM_CollectionOfMSEs REF Collection,
  [out] CIM_ConcreteJob      REF Job
);
```



## Parameters

<dl> <dt>

*Collection* \[in\]
</dt> <dd>

The collection to destroy.

</dd> <dt>

*Job* \[out\]
</dt> <dd>

A reference to the job (can be null if the task is completed).

</dd> </dl>

## Return value

Returns 0 if successful, or 4096 if the job started; otherwise, returns an error.

<dl> <dt>

**Completed with No Error** (0)
</dt> <dt>

**Method Parameters Checked - Job Started** (4096)
</dt> <dt>

**Failed** (32768)
</dt> <dt>

**Access Denied** (32769)
</dt> <dt>

**Not Supported** (32770)
</dt> <dt>

**Status is unknown** (32771)
</dt> <dt>

**Timeout** (32772)
</dt> <dt>

**Invalid parameter** (32773)
</dt> <dt>

**System is in use** (32774)
</dt> <dt>

**Invalid state for this operation** (32775)
</dt> <dt>

**Incorrect data type** (32776)
</dt> <dt>

**System is not available** (32777)
</dt> <dt>

**Out of memory** (32778)
</dt> <dt>

**File not found** (32779)
</dt> </dl>

## Requirements



| Requirement | Value |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 10 \[desktop apps only\]<br/>                                                             |
| Minimum supported server<br/> | Windows Server 2016<br/>                                                                          |
| Namespace<br/>                | Root\\virtualization\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## See also

<dl> <dt>

[**Msvm\_CollectionManagementService**](msvm-collectionmanagementservice.md)
</dt> </dl>

 

 




