---
title: "Compiler Error CS0514"
ms.custom: na
ms.date: 10/01/2016
ms.devlang: 
  - CSharp
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 74ce3010-f9e9-458c-8b68-cfb908a3e7a2
caps.latest.revision: 10
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
# Compiler Error CS0514
'constructor' : static constructor cannot have an explicit 'this' or 'base' constructor call  
  
 Calling `this` in the static constructor is not allowed because the static constructor is called automatically before creating any instance of the class. Also, static constructors are not inherited, and cannot be called directly.  
  
 For more information, see [this](../Topic/this%20\(C%23%20Reference\).md) and [base](../Topic/base%20\(C%23%20Reference\).md).  
  
## Example  
 The following example generates CS0514:  
  
```  
// CS0514.cs  
class A  
{  
    static A() : base(0) // CS0514  
    {  
    }  
  
    public A(object o)  
    {  
    }  
}  
  
class B  
{  
    static B() : this(null) // CS0514  
    {  
    }  
  
    public B(object o)  
    {  
    }  
}  
```