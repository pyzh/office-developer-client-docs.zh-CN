---
title: 单元格元素 （RelQuadBezTo 行） (Visio XML)
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8b3aea70-a69f-a85e-83d8-c0fa2ee68836
description: 包含 x 坐标或 y 坐标的相对于形状的宽度和高度二次贝塞尔曲线的终结点或曲线相对于形状的宽度和高度的控制点 x 或 y 坐标。
ms.openlocfilehash: 5f823e5930d3dad8bf6e20727e4b527493f89892
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19779852"
---
# <a name="cell-element-relquadbezto-row-visio-xml"></a>单元格元素 （RelQuadBezTo 行） (Visio XML)

包含 x 坐标或 y 坐标的相对于形状的宽度和高度二次贝塞尔曲线的终结点或曲线相对于形状的宽度和高度的控制点 x 或 y 坐标。
  
## <a name="element-information"></a>元素信息

|||
|:-----|:-----|
|**元素类型** <br/> |[Cell_Type](cell_type-complextypevisio-xml.md) <br/> |
|**命名空间** <br/> |http://schemas.microsoft.com/office/visio/2012/main  <br/> |
|**架构文件** <br/> |VisioSchema15.xsd  <br/> |
|**文档部件** <br/> |母版页 #.xml、 页面 #.xml  <br/> |
   
## <a name="definition"></a>定义

```XML
< xs:element name="Cell" type="Cell_Type" minOccurs="0" maxOccurs="unbounded" >
</xs:element >
```

## <a name="elements-and-attributes"></a>元素和属性

### <a name="parent-elements"></a>父元素

|**元素**|**类型**|**说明**|
|:-----|:-----|:-----|
|[Row 元素 （geometry)](row-element-geometry-sectionvisio-xml.md) <br/> |[RelQuadBezTo_Type](relquadbezto_type-complextypevisio-xml.md) <br/> |包含 x 坐标或 y 坐标的相对于形状的宽度和高度二次贝塞尔曲线的终结点或曲线相对于形状的宽度和高度的控制点 x 或 y 坐标。  <br/> |
   
### <a name="child-elements"></a>子元素

|**元素**|**类型**|**说明**|
|:-----|:-----|:-----|
|[RefBy](refby-element-cell_type-complextypevisio-xml.md) <br/> |[RefBy_Type](refby_type-complextypevisio-xml.md) <br/> |指定在绘图页上的引用。  <br/> |
   
### <a name="attributes"></a>Attributes

|**属性**|**类型**|**必需**|**说明**|**可能的值**|
|:-----|:-----|:-----|:-----|:-----|
|E  <br/> |xsd: string  <br/> |可选  <br/> |指示该公式计算为错误。 **E**的值是当前值 （错误消息字符串）;**V**属性的值是最后一个有效的值。  <br/> |错误消息字符串。  <br/> |
|F  <br/> |xsd: string  <br/> |可选  <br/> | 代表元素的公式。 此属性可以包含以下字符串之一：  <br/>  （某些公式） 如果公式本地存在  <br/>  `No Formula`如果本地删除或阻止公式  <br/>  `Inh`如果继承的公式。  <br/> |公式。  <br/> |
|N  <br/> |xsd: string  <br/> |必需  <br/> |表示的 ShapeSheet 单元格的名称。  <br/> |ShapeSheet 单元格的名称。  <br/> 请参阅下面的备注部分。  <br/> |
|U  <br/> |xsd: string  <br/> |可选  <br/> |代表单位默认值是度量的 DL。  <br/> |单元格的单位。  <br/> |
|V  <br/> |xsd: string  <br/> |可选  <br/> |代表单元格的值。  <br/> |ShapeSheet 单元格的值。  <br/> |
   
## <a name="remarks"></a>说明

此**单元格**元素的**N**属性必须为一组有限的对应于 ShapeSheet 单元格的值之一。 请参阅下表为确定允许此**单元格**元素的**N**属性的值。 
  
|**值**|**说明**|**更多信息**|
|:-----|:-----|:-----|
|X  <br/> |终顶点相对于形状的宽度二次贝塞尔曲线的 x 轴坐标值。  <br/> |[RelQuadBezTo 行（“Geometry”部分）](relquadbezto-row-geometry-section.md) <br/> |
|Y  <br/> |终顶点相对于形状的高度二次贝塞尔曲线的 y 轴坐标值。  <br/> |[RelQuadBezTo 行（“Geometry”部分）](relquadbezto-row-geometry-section.md) <br/> |
|A  <br/> |相对于形状的宽度; 控制点的位于曲线的控件的 x 坐标弧形上某个点。是最好位于之间的开始和结束顶点的一半的控制点。  <br/> |[RelQuadBezTo 行（“Geometry”部分）](relquadbezto-row-geometry-section.md) <br/> |
|B  <br/> |相对于形状的高度控制点曲线的控件的 y 坐标。  <br/> |[RelQuadBezTo 行（“Geometry”部分）](relquadbezto-row-geometry-section.md) <br/> |
   

