---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: L’élément DeliverMeetingRequests définit la façon dont les demandes de réunion sont gérées entre le délégué et le principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 8e61af87337cb1fc8936b4de7753fca2d6c1161e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519827"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

**L’élément DeliverMeetingRequests** définit la façon dont les demandes de réunion sont gérées entre le délégué et le principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Définit une demande d’ajout de délégués à une boîte aux lettres. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Définit une demande de mise à jour des délégués dans une boîte aux lettres. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Contient l’état et le résultat d’une demande GetDelegate. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément DeliverMeetingRequests.** 
  
**Valeurs de l’élément DeliverMeetingRequests**

|**Valeur**|**Description**|
|:-----|:-----|
|DelegatesOnly  <br/> |Les demandes de réunion sont transférés au délégué et déplacés vers le dossier Éléments supprimés de la boîte aux lettres du principal.  <br/> |
|DelegatesAndMe  <br/> |Les demandes de réunion sont transmis au délégué et restent dans le dossier Boîte de réception de la boîte aux lettres du principal.  <br/> |
|DelegatesAndSendInformationToMe  <br/> |Les demandes de réunion sont transmis au délégué et restent dans le dossier Boîte de réception de la boîte aux lettres du principal, mais les boutons Accepter, Provisoire et Refuser n’apparaissent pas dans le volet de lecture Microsoft Office Outlook.  <br/> |
|NoForward  <br/> |Les demandes de réunion ne sont pas transmis au délégué.  <br/> |
   
## <a name="remarks"></a>Remarques

Le **paramètre DeliverMeetingRequests affecte** tous les délégués de la boîte aux lettres d’un principal. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md)  
- [Opération UpdateDelegate](updatedelegate-operation.md)  
- [Opération GetDelegate](getdelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

