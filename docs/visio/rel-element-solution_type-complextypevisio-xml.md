---
title: Rel 元素 （Solution_Type 复杂类型） (Visio XML)
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8438fe4b-f5f7-d4e4-58b7-7ebdc1da197a
description: 指定与此解决方案的 XML 关联的解决方案与部件的关系。
ms.openlocfilehash: 59d9db3f7e0897abf278a27229c07fd3942cee79
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19781042"
---
# <a name="rel-element-solutiontype-complextype-visio-xml"></a>Rel 元素 （Solution_Type 复杂类型） (Visio XML)

指定与此解决方案的 XML 关联的解决方案与部件的关系。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|**元素类型** <br/> |[Rel_Type](rel_type-complextypevisio-xml.md) <br/> |
|**命名空间** <br/> |http://schemas.microsoft.com/office/visio/2012/main  <br/> |
|**架构文件** <br/> |VisioSchema15.xsd  <br/> |
|**文档部件** <br/> |pages.xml、 masters.xml、 recordsets.xml、 页 #.xml、 主 #.xml  <br/> |
   
## <a name="definition"></a>定义

```XML
<xs:element name="Rel" type="Rel_Type" minOccurs="1" maxOccurs="1" >
</xs:element>
```

## <a name="elements-and-attributes"></a>元素和属性

如果此架构定义了具体要求，如**sequence**， **minOccurs**、 **maxOccurs**和**choice**，请参阅定义部分。 
  
### <a name="parent-elements"></a>父元素

|**元素**|**类型**|**说明**|
|:-----|:-----|:-----|
|[Solution](solution-element-solutions_type-complextypevisio-xml.md) <br/> |[Solution_Type](solution_type-complextypevisio-xml.md) <br/> |指定 XML 存储在绘图中的解决方案的一个的实例。  <br/> |
   
### <a name="child-elements"></a>子元素

无。
  
### <a name="attributes"></a>属性

|**属性**|**类型**|**必需**|**说明**|**可能的值**|
|:-----|:-----|:-----|:-----|:-----|
|r: id  <br/> |xsd: string  <br/> 请参阅注解。  <br/> |必需  <br/> |指定与部件的关系。  <br/> |"删除 #"  <br/> 请参阅注解。  <br/> |
   
## <a name="remarks"></a>说明

**R: id**属性的值必须是**ST_RelationshipID**类型。 **ST_RelationshipID**类型是一个 string 类型的值必须是格式为删除的 #，最后一个字符必须数字。 号码必须是唯一的**Rel**元素的所有同级元素。 
  
有关 ST_RelationshipID 类型的详细信息，请参阅[第 1 部分 ISO/IEC 29500 规范](http://www.iso.org/iso/home/store/catalogue_tc/catalogue_detail.md?csnumber=61750)。
  

