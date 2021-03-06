---
title: IMAPIFormContainerRemoveForm
manager: soliver
ms.date: 03/09/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IMAPIFormContainer.RemoveForm
api_type:
- COM
ms.assetid: 7f851ce8-bd01-4ea5-86e0-e44323cc0aab
description: 上次修改时间：2015 年 3 月 9 日
ms.openlocfilehash: 0d2c908f86ccd66ffd3a2eb2506d129ee2a14d48
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19775388"
---
# <a name="imapiformcontainerremoveform"></a>IMAPIFormContainer::RemoveForm

  
  
**适用于**： Outlook 
  
从窗体容器中删除特定的窗体。
  
```cpp
HRESULT RemoveForm(
  LPCSTR szMessageClass
);
```

## <a name="parameters"></a>参数

 _szMessageClass_
  
> [in]命名窗体，从窗体容器中删除的邮件类的字符串。 邮件类名称始终都是 ANSI 字符串，从不 Unicode。
    
## <a name="return-value"></a>返回值

S_OK 
  
> 呼叫成功或多个预期值返回。
    
MAPI_E_NOT_FOUND 
  
> _SzMessageClass_参数中传递的邮件类不匹配窗体容器中的任何窗体的邮件类。 
    
## <a name="mfcmapi-reference"></a>MFCMAPI 参考 （英文）

MFCMAPI 示例代码，请参阅下表。
  
|**文件**|**函数**|**Comment**|
|:-----|:-----|:-----|
|FormContainerDlg.cpp  <br/> |CFormContainerDlg::OnDeleteSelectedItem  <br/> |MFCMAPI 使用**IMAPIFormContainer::RemoveForm**方法从窗体容器中删除窗体。  <br/> |
   
## <a name="see-also"></a>另请参阅



[IMAPIFormContainer : IUnknown](imapiformcontaineriunknown.md)


[MFCMAPI 代码示例](mfcmapi-as-a-code-sample.md)

