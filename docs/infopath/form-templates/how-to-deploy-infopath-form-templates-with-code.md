---
title: 部署包含代码的 InfoPath 表单模板
manager: soliver
ms.date: 11/16/2014
ms.audience: Developer
keywords:
- deploying form templates [infopath 2007],InfoPath 2007, deploying form templates,form templates [InfoPath 2007], deploying,.NET Framework security settings [InfoPath 2007],deployment [InfoPath 2007], form templates
localization_priority: Normal
ms.assetid: ab66e26d-74ee-4211-b387-1385183a6803
description: InfoPath 托管代码表单模板的表单代码编译为在公共语言运行库 (CLR) 下运行的程序集。这意味着只要您需要对表单代码进行更改，就必须在 Visual Studio 2008 中打开其项目，在代码编辑器中进行更改，重新编译表单模板，然后重新部署该表单模板。此外，由于托管代码表单模板的专用程序集是在托管的 CLR 应用程序域中运行的，因此需要完全信任的表单的安全设置与不需要完全信任的表单模板稍有不同。
ms.openlocfilehash: 56af865a80df75c7e1d973767066a03310cdde1e
ms.sourcegitcommit: 9d60cd82b5413446e5bc8ace2cd689f683fb41a7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2018
ms.locfileid: "19773981"
---
# <a name="deploy-infopath-form-templates-with-code"></a>部署包含代码的 InfoPath 表单模板

InfoPath 托管代码表单模板的表单代码编译为在公共语言运行库 (CLR) 下运行的程序集。这意味着只要您需要对表单代码进行更改，就必须在 Visual Studio 2008 中打开其项目，在代码编辑器中进行更改，重新编译表单模板，然后重新部署该表单模板。此外，由于托管代码表单模板的专用程序集是在托管的 CLR 应用程序域中运行的，因此需要完全信任的表单的安全设置与不需要完全信任的表单模板稍有不同。
  
## <a name="deploying-form-templates-that-do-not-require-full-trust"></a>部署不需要完全信任的表单模板

如果您的表单模板的表单代码不使用需要完全信任的 InfoPath 对象模型成员，并且该表单模板不使用需要完全信任的功能，那么您可以使用以下步骤直接从 InfoPath 发布您的表单模板。有关 InfoPath 安全模型的信息，请参阅[关于具有代码的表单模板的安全模型](about-the-security-model-for-form-templates-with-code.md)。
  
### <a name="deploy-a-form-template-that-does-not-require-full-trust"></a>部署不需要完全信任的表单模板

1. 在 Visual Studio 2008 中创建和调试表单模板。
    
2. 如果你在 Visual Studio 2012 代码编辑器中工作，请切换到 InfoPath，单击“文件”**** 选项卡，然后在“发布”**** 选项卡上单击所需发布位置的按钮。（如果之前已发布该表单模板，则可单击“文件”**** 选项卡，再单击“快速发布”**** 将该表单模板重新发布到同一位置。） 
    
    将编译表单模板并启动“发布向导”****。 按照“发布向导”**** 中的步骤将你的表单部署到你所选的位置。 有关使用“发布向导”**** 的详细信息，请搜索“发布表单模板”的 InfoPath 帮助。
    
## <a name="deploying-form-templates-that-require-full-trust"></a>部署需要完全信任的表单模板

如果您的表单模板的表单代码使用需要完全信任的 InfoPath 对象模型成员，或者该表单模板使用需要完全信任的功能，则您必须使用来自受信任发布者的代码签名证书对您的表单模板 (.xsn) 文件进行数字签名，当您的用户打开表单时，系统将提示他们信任该证书。这将使您的表单完全受信任，反过来也对您的表单代码授予 FullTrust 权限集。
  
### <a name="compile-publish-and-digitally-sign-a-form-template"></a>编译、发布表单模板并对其进行数字签名

1. 在 Visual Studio 2008 中创建和调试表单模板。
    
2. 如果你在 Visual Studio 2012 代码编辑器中工作，请切换到 InfoPath，然后依次单击“文件”**** 选项卡和“表单选项”****。
    
3. 单击“安全和信任”**** 类别。 
    
4. 在“安全级别”**** 下，清除“自动确定安全级别”**** 复选框，然后选择“完全信任”****。
    
5. 在“表单模板签名”**** 下，选择“为此表单模板签名”****，单击“选择证书”****，然后指定用于对表单模板进行签名的代码签名证书。
    
6. 单击“确定”**** 两次以关闭“表单选项”**** 对话框，然后保存所做的更改。 
    
7. 单击“发布”**** 选项卡，然后单击所需的发布位置的按钮。 
    
8. 将编译表单模板并启动“发布向导”****。 按照“发布向导”**** 中的步骤来部署你的表单模板。 有关使用“发布向导”**** 来部署需要完全信任的表单模板的详细信息，请搜索“发布包含完全信任的表单模板”的 InfoPath 帮助。 
    
 **备注**
- 要对表单进行数字签名，计算机上必须安装了经过验证的代码签名证书。要获取这样的证书，必须与证书颁发机构或网络管理员联系。
    
- 如果需要在发布表单后对其进行更改，必须重复该步骤并重新签名表单模板。 这是因为更改表单将使数字签名无效。 在开发需要完全信任权限的表单的过程中，可以使用[预览和调试需要完全信任的表单模板](how-to-preview-and-debug-form-templates-that-require-full-trust.md)中介绍的过程在你的本地计算机上注册表单模板。 
    
## <a name="configuring-net-framework-security-settings"></a>配置 .NET Framework 安全设置

要对授予在 InfoPath 托管代码表单模板中运行的托管代码的权限进行更多控制，可以使用 .NET Framework 2.0 配置实用程序对您的表单代码授予特定权限集。
  
> [!IMPORTANT]
> 为 InfoPath 托管代码表单模板配置 .NET Framework 安全设置时，不会影响是否允许运行需要完全信任的 InfoPath 对象模型成员。您必须按照本主题前面所述的过程对表单模板进行数字签名或注册，以允许调用需要完全信任的 InfoPath 对象模型成员。配置 .NET Framework 安全设置仅适用于对 .NET Framework 类的成员和托管组件的调用，而不适用于 InfoPath 对象模型。 
  
### <a name="compile-publish-and-configure-net-security-settings-for-a-form-template"></a>编译、发布和配置表单模板的 .NET 安全设置

1. 在 Visual Studio 2008 中创建和调试表单模板。
    
2. 如果你在 Visual Studio 2012 代码编辑器中工作，请切换到 InfoPath，依次单击“文件”**** 选项卡和“发布”****，然后单击所需发布位置的按钮。
    
    将编译表单模板并启动“发布向导”****。 按照“发布向导”**** 中的步骤来部署你的表单模板。 有关使用“发布向导”**** 的详细信息，请搜索“发布表单模板”的 InfoPath 帮助。
    
3. 执行[为包含代码的表单模板配置安全设置](how-to-configure-security-settings-for-form-templates-with-code.md)的“为位于特定 URL 或 UNC 的表单指定 FullTrust”一节中所述的步骤。
    
## <a name="see-also"></a>另请参阅

#### <a name="tasks"></a>任务

[为包含代码的表单模板配置安全设置](how-to-configure-security-settings-for-form-templates-with-code.md)


[有关包含代码的表单模板的安全模型](about-the-security-model-for-form-templates-with-code.md)
  
[预览和调试需要完全信任的表单模板](how-to-preview-and-debug-form-templates-that-require-full-trust.md)

