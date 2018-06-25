---
title: Utilisateur_délégué
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: L’élément Utilisateur_délégué identifie un seul délégué pour ajouter ou mettre à jour dans une boîte aux lettres ou un délégué renvoyés dans une réponse de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755838"
---
# <a name="delegateuser"></a>Utilisateur_délégué

L’élément **Utilisateur_délégué** identifie un seul délégué pour ajouter ou mettre à jour dans une boîte aux lettres ou un délégué renvoyés dans une réponse de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

**DelegateUserType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom d’utilisateur](userid.md) <br/> |Identifie le délégué. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[DelegatePermissions](delegatepermissions.md) <br/> |Contient les paramètres de niveau d’autorisation délégué. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ReceiveCopiesOfMeetingMessages](receivecopiesofmeetingmessages.md) <br/> |Indique si un délégué reçoive des copies de messages adressés à l’entité de sécurité liées à la réunion. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Indique si un délégué a l’autorisation d’afficher des éléments de calendrier privés de boîte aux lettres de l’entité de sécurité. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |Contient les identités des délégués pour ajouter ou mettre à jour dans une boîte aux lettres.  <br/> |
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contient des messages de réponse pour les opérations de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md) 
- [Opération UpdateDelegate](updatedelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

