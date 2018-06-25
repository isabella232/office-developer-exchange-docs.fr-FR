---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: L’élément DeliverMeetingRequests définit la gestion des demandes de réunion entre le délégué et l’entité de sécurité. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755889"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

L’élément **DeliverMeetingRequests** définit la gestion des demandes de réunion entre le délégué et l’entité de sécurité. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Définit une demande pour ajouter des délégués à une boîte aux lettres. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Définit une demande de mise à jour des délégués dans une boîte aux lettres. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’état et les résultats d’une demande GetDelegate. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **DeliverMeetingRequests** . 
  
**Valeurs des éléments DeliverMeetingRequests**

|**Valeur**|**Description**|
|:-----|:-----|
|DelegatesOnly  <br/> |Demandes de réunion sont transmises au délégué et déplacés vers le dossier éléments supprimés dans la boîte aux lettres de l’entité de sécurité.  <br/> |
|DelegatesAndMe  <br/> |Demandes de réunion sont transférés vers le délégué et restent dans le dossier boîte de réception dans la boîte aux lettres de l’entité de sécurité.  <br/> |
|DelegatesAndSendInformationToMe  <br/> |Demandes de réunion sont transférés vers le délégué et restent dans le dossier boîte de réception dans la boîte aux lettres de l’entité de sécurité, mais les boutons Accepter, provisoire et refuser n’apparaissent pas dans le volet de lecture de Microsoft Office Outlook.  <br/> |
|NoForward  <br/> |Demandes de réunion ne sont pas transférés vers le délégué.  <br/> |
   
## <a name="remarks"></a>Remarques

Le paramètre **DeliverMeetingRequests** affecte tous les délégués dans la boîte aux lettres d’un utilisateur principal. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md)  
- [Opération UpdateDelegate](updatedelegate-operation.md)  
- [Opération GetDelegate](getdelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

