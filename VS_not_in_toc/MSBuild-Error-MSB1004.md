---
title: "MSBuild Error MSB1004"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: aed36761-ab07-486c-b5eb-48ccb1c387dd
caps.latest.revision: 12
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# MSBuild Error MSB1004
**Specify the name of the target.**  
  
 At least one target must be specified with the **/target** switch.  
  
### To correct this error  
  
1.  Specify a target or targets. You can use either a comma or a semicolon to separate a list of targets, for example, `/target:Clean;Compile`. Alternatively, you can repeat the switch, for example, `/t:Clean /t:``Compile`  
  
## See Also  
 [Targets](../VS_IDE/MSBuild-Targets.md)   
 [Command-Line Reference](../VS_IDE/MSBuild-Command-Line-Reference.md)