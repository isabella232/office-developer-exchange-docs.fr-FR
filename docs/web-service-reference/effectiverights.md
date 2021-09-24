---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: L’élément EffectiveRights contient les droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier. Cet élément est en lecture seule.
ms.openlocfilehash: a3207a9971065d3b69b6a0b7056fa8012425fd5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514710"
---
# <a name="effectiverights"></a>EffectiveRights

**L’élément EffectiveRights** contient les droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier. Cet élément est en lecture seule. 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 **EffectiveRightsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CreateAssociated](createassociated.md) <br/> |Indique si un client peut créer une table des matières associée. Cette propriété est utilisée uniquement sur les objets de dossier.  <br/> |
|[CreateContents](createcontents.md) <br/> |Indique si un client peut créer une table des matières. Cette propriété est utilisée uniquement sur les objets de dossier.  <br/> |
|[CreateHierarchy](createhierarchy.md) <br/> |Indique si un client peut créer une table hiérarchique. Cette propriété est utilisée uniquement sur les objets de dossier.  <br/> |
|[Supprimer](delete.md) <br/> |Indique si un client peut supprimer un dossier ou un élément.  <br/> |
|[Modify](modify.md) <br/> |Indique si un client peut modifier un dossier ou un élément.  <br/> |
|[Read](read.md) <br/> |Indique si un client peut lire un dossier ou un élément.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Indique si un élément privé peut être vu.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Représente un dossier dans une boîte aux lettres.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier de tâches dans une boîte aux lettres.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier de calendrier dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche dans une boîte aux lettres.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément Exchange générique.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément de publication dans la Exchange store.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

**EffectiveRights est** pris en charge dans les réponses GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy et SyncFolderItems. La **propriété EffectiveRights** est exposée dans la forme **AllProperties** pour les dossiers et les éléments. 
  
Cette **propriété EffectiveRights** permet d’accéder aux mêmes informations que dans la **PR_ACCESS MAPI.** 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

