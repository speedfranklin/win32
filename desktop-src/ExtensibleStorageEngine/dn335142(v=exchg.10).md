---
title: JET_ENUMCOLUMNVALUE class (Microsoft.Isam.Esent.Interop)
TOCTitle: JET_ENUMCOLUMNVALUE class
ms:assetid: T:Microsoft.Isam.Esent.Interop.JET_ENUMCOLUMNVALUE
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.jet_enumcolumnvalue(v=EXCHG.10)
ms:contentKeyID: 55103622
ms.date: 07/30/2014
mtps_version: v=EXCHG.10
f1_keywords:
- Microsoft.Isam.Esent.Interop.JET_ENUMCOLUMNVALUE
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.JET_ENUMCOLUMNVALUE
topic_type: 
- kbSyntax
- apiref
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# JET\_ENUMCOLUMNVALUE class

Enumerates the column values of a record using the JetEnumerateColumns function. [JetEnumerateColumns(JET\_SESID, JET\_TABLEID, Int32, \[\], Int32, \[\], JET\_PFNREALLOC, IntPtr, Int32, EnumerateColumnsGrbit)](dn292148\(v=exchg.10\).md) returns an array of JET\_ENUMCOLUMNVALUE structures. The array is returned in memory that was allocated using the callback that was supplied to that function.

## Inheritance hierarchy

[System.Object](http://msdn2.microsoft.com/en-us/library/e5kfa45b)  
  Microsoft.Isam.Esent.Interop.JET\_ENUMCOLUMNVALUE  

**Namespace:**  [Microsoft.Isam.Esent.Interop](hh596136\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Class JET_ENUMCOLUMNVALUE
'Usage
Dim instance As JET_ENUMCOLUMNVALUE
```

``` csharp
public class JET_ENUMCOLUMNVALUE
```

## Thread safety

Any public static (Shared in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.

## See also

#### Reference

[JET\_ENUMCOLUMNVALUE members](dn335094\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop namespace](hh596136\(v=exchg.10\).md)
