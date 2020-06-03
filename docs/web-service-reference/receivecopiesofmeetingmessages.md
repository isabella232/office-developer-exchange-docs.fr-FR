---
title: ReceiveCopiesOfMeetingMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: L’élément ReceiveCopiesOfMeetingMessages indique si un délégué reçoit des copies des messages relatifs à la réunion adressés au principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: af6e220304f88c4db00ab675077dcd9bf581ea9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468263"
---
# <a name="receivecopiesofmeetingmessages"></a>ReceiveCopiesOfMeetingMessages

L’élément **ReceiveCopiesOfMeetingMessages** indique si un délégué reçoit des copies des messages relatifs à la réunion adressés au principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Identifie un seul délégué à ajouter ou mettre à jour dans une boîte aux lettres. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** indique qu’un délégué reçoit une copie des messages de réunion. Une valeur de texte **false** indique qu’un délégué ne reçoit pas de copie des messages de réunion. 
  
## <a name="remarks"></a>Remarques

Lorsque **ReceiveCopiesOfMeetingMessages** est défini sur **false**, le délégué peut toujours envoyer un message de la part du principal, mais ne reçoit pas de messages liés à la réunion.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

