---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: L’élément RightsManagementLicenseData spécifie des informations sur la licence de gestion des droits pour un élément.
ms.openlocfilehash: 892edfd6775838b1e6329e8db0ee9bb8e3c519ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463187"
---
# <a name="rightsmanagementlicensedata"></a>RightsManagementLicenseData

L’élément **RightsManagementLicenseData** spécifie des informations sur la licence de gestion des droits pour un élément. 
  
```XML
<RightsManagementLicenseData>
   <RightsManagedMessageDecryptionStatus/>
   <RmsTemplateId/>
   <TemplateName/>
   <TemplateDescription/>
   <EditAllowed/>
   <ReplyAllowed/>
   <ReplyAllAllowed/>
   <ForwardAllowed/>
   <ModifyRecipientsAllowed/>
   <ExtractAllowed/>
   <PrintAllowed/>
   <ExportAllowed/>
   <ProgrammaticAccessAllowed/>
   <IsOwner/>
   <ContentOwner/>
   <ContentExpiryDate/>
</RightsManagementLicenseData>
```

 **RightsManagementLicenseDataType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md)  |  [RMSTemplateId](rmstemplateid.md)  |  [TemplateName](templatename.md)  |  [TemplateDescription](templatedescription.md)  |  [EditAllowed](editallowed.md)  |  [ReplyAllowed](replyallowed.md)  |  [ReplyAllAllowed](replyallallowed.md)  |  [ForwardAllowed](forwardallowed.md)  |  [ModifyRecipientsAllowed](modifyrecipientsallowed.md)  |  [ExtractAllowed](extractallowed.md)  |  [PrintAllowed](printallowed.md)  |  [ExportAllowed](exportallowed.md)  |  [ProgrammaticAccessAllowed](programmaticaccessallowed.md)  |  [IsOwner](isowner.md)  |  [ContentOwner](contentowner.md)  |  [ContentExpiryDate](contentexpirydate.md)
  
### <a name="parent-elements"></a>Éléments parents

[Élément](item.md)  |  [Message](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [Propriété meetingrequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tâche](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

