---
title: "Publish Page, Project Designer"
ms.custom: na
ms.date: 10/06/2016
ms.devlang: 
  - VB
  - CSharp
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - vs-ide-general
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 153527c6-8b95-4003-8e8e-03a489d0a629
caps.latest.revision: 33
manager: ghogen
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
# Publish Page, Project Designer
The **Publish** page of the **Project Designer** is used to configure properties for ClickOnce deployment.  
  
 To access the **Publish** page, select a project node in **Solution Explorer**, and then, on the **Project** menu, click **Properties**. When the **Project Designer** appears, click the **Publish** tab.  
  
> [!NOTE]
>  Some of the ClickOnce properties described here can also be set in the **PublishWizard**, available from the **Build** menu or by clicking the **PublishWizard** button on this page.  
  
## UIElement List  
 **Publishing Folder Location**  
 Specifies the location where the application is published. Can be a drive path (`C:\deploy\myapplication`), a file share (`\\server\myapplication`), an FTP server (`ftp://ftp.microsoft.com/myapplication`), or a Web site (`http://www.microsoft.com/myapplication`). Note that text must be present in the **Publishing Location** box in order for the browse (**...**) button to work.  
  
 By default, the publishing location is `http://localhost/<projectname>/` if you have IIS installed, or the `publish\` directory if you do not have IIS installed. If your computer is running Windows Vista, the default is always the `publish\` directory, regardless of whether you have IIS installed.  
  
 **Installation Folder URL**  
 Optional. Specifies a Web site to which users go to install the application. This is necessary only when it differs from the **Publishing Location**, for example, when the application is published to a staging server.  
  
 **Install Mode and Settings**  
 Determines whether the application is run directly from the **Publishing Location** (when **The application is available online only** is selected) or is installed and added to the **Start** menu and the **Add or Remove Programs** item in **Control Panel** (when **The application is available offline as well** is selected).  
  
 For WPF Web Browser Applications, the **The application is available offline as well** option is disabled, because such applications are available only online.  
  
 **Application Files**  
 Opens the [Application Files Dialog Box](assetId:///b06dff3a-b87a-4caf-996b-7a4acf8137a8), which is used to specify how and where individual files are installed.  
  
 **Prerequisites**  
 Opens the [Prerequisites Dialog Box](../VS_IDE/Prerequisites-Dialog-Box.md), which is used to specify prerequisite components, such as the .NET Framework, to be installed together with the application.  
  
 **Updates**  
 Opens the [Application Updates Dialog Box](assetId:///8eca8743-8e68-4d04-bfd5-4dc0a9b2934f), which is used to specify update behavior for the application. Not available when **The application is available online only** is selected.  
  
 **Options**  
 Opens the [Publish Options Dialog Box](assetId:///fd9baa1b-7311-4f9e-8ffb-ae50cf110592), which is used to specify additional advanced publishing options.  
  
 **Publish Version**  
 Sets the publish version number for the application; when the version number is changed, the application is published as an update. Each part of the publish version (**Major**, **Minor**, **Build**, **Revision**) can have a maximum value of 65355 (<xref:System.UInt16.MaxValue?qualifyHint=False>), the maximum allowed by <xref:System.Version?qualifyHint=False>.  
  
 When you install more than one version of an application by using ClickOnce, the installation moves earlier versions of the application into a folder named Archive, in the publish location that you specify. Archiving earlier versions in this manner keeps the installation directory clear of folders from the earlier version.  
  
 **Automatically increment revision with each publish**  
 Optional. When this option is selected (the default), the **Revision** part of the publish version number is incremented by one every time that the application is published. This causes the application to be published as an update.  
  
 **Publish Wizard**  
 Opens the [Publish Wizard](assetId:///fc6abebd-13d6-48e4-a567-fbc52dad0872). Completing the Publish Wizard has the same effect as running the **Publish** command on the **Build** menu.  
  
 **Publish Now**  
 Publishes the application using the current settings. Equivalent to the **Finish** button in the **PublishWizard**.  
  
## See Also  
 [Publishing ClickOnce Applications](../VS_IDE/Publishing-ClickOnce-Applications.md)   
 [How to: Publish a ClickOnce Application using the Publish Wizard](../VS_IDE/How-to--Publish-a-ClickOnce-Application-using-the-Publish-Wizard.md)   
 [How to: Specify Where Visual Studio Copies the Files](../VS_IDE/How-to--Specify-Where-Visual-Studio-Copies-the-Files.md)   
 [How to: Specify the Location Where End Users Will Install From](../VS_IDE/How-to--Specify-the-Location-Where-End-Users-Will-Install-From.md)   
 [How to: Specify a Link for Technical Support](../VS_IDE/How-to--Specify-a-Link-for-Technical-Support.md)   
 [How to: Specify the ClickOnce Offline or Online Install Mode](../VS_IDE/How-to--Specify-the-ClickOnce-Offline-or-Online-Install-Mode.md)   
 [How to: Enable AutoStart for CD Installations](../VS_IDE/How-to--Enable-AutoStart-for-CD-Installations.md)   
 [How to: Set the ClickOnce Publish Version](../VS_IDE/How-to--Set-the-ClickOnce-Publish-Version.md)   
 [How to: Automatically Increment the ClickOnce Publish Version](../VS_IDE/How-to--Automatically-Increment-the-ClickOnce-Publish-Version.md)   
 [How to: Specify Which Files Are Published by ClickOnce](../VS_IDE/How-to--Specify-Which-Files-Are-Published-by-ClickOnce.md)   
 [How to: Install Prerequisites with a ClickOnce Application](../VS_IDE/How-to--Install-Prerequisites-with-a-ClickOnce-Application.md)   
 [How to: Manage Updates for a ClickOnce Application](../VS_IDE/How-to--Manage-Updates-for-a-ClickOnce-Application.md)   
 [How to: Change the Publish Language for a ClickOnce Application](../VS_IDE/How-to--Change-the-Publish-Language-for-a-ClickOnce-Application.md)   
 [How to: Specify a Start Menu Name for a ClickOnce Application](../VS_IDE/How-to--Specify-a-Start-Menu-Name-for-a-ClickOnce-Application.md)   
 [How to: Specify a Publish Page for a ClickOnce Application](../VS_IDE/How-to--Specify-a-Publish-Page-for-a-ClickOnce-Application.md)   
 [ClickOnce Security and Deployment](../VS_IDE/ClickOnce-Security-and-Deployment.md)