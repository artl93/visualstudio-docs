---
title: "&#39;&lt;elementname&gt;&#39; is obsolete: &#39;&lt;errormessage&gt;&#39;"
ms.custom: na
ms.date: "10/13/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-csharp"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "bc40000"
  - "vbc40000"
helpviewer_keywords: 
  - "BC40000"
ms.assetid: dade0f57-eca1-4dd0-b978-020678838be6
caps.latest.revision: 12
ms.author: "billchi"
manager: "douge"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# &#39;&lt;elementname&gt;&#39; is obsolete: &#39;&lt;errormessage&gt;&#39;
A statement attempts to access a programming element which has been marked with the \<xref:System.ObsoleteAttribute> attribute and the directive to treat it as a warning.  
  
 You can mark any programming element as being no longer in use by applying \<xref:System.ObsoleteAttribute> to it. If you do this, you can set the attribute's \<xref:System.ObsoleteAttribute.IsError*> property to either `True` or `False`. If you set it to `True`, the compiler treats an attempt to use the element as an error. If you set it to `False`, or let it default to `False`, the compiler issues a warning if there is an attempt to use the element.  
  
 By default, this message is a warning, because the \<xref:System.ObsoleteAttribute.IsError*> property of \<xref:System.ObsoleteAttribute> is `False`. For more information about hiding warnings or treating warnings as errors, see [Configuring Warnings in Visual Basic](../ide/configuring-warnings-in-visual-basic.md).  
  
 **Error ID:** BC40000  
  
### To correct this error  
  
1.  Examine the quoted error message and take appropriate action.  
  
2.  Ensure that the source code reference is spelling the element name correctly.  
  
## See Also  
 [NOT IN BUILD: Attributes Used in Visual Basic](assetId:///22231318-8a40-49af-9245-e0aab723563b)   
 [NOT IN BUILD: Application of Attributes](assetId:///2b1703ed-4437-49b3-bc0b-568094324f47)