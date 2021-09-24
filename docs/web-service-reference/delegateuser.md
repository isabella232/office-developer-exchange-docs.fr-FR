---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: L’élément DelegateUser identifie un délégué unique à ajouter ou à mettre à jour dans une boîte aux lettres ou un délégué renvoyé dans une réponse de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 1963bef64e32ff536f0544a03f019e7785bae4d0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510254"
---
# <a name="delegateuser"></a>DelegateUser

**L’élément DelegateUser** identifie un délégué unique à ajouter ou à mettre à jour dans une boîte aux lettres ou un délégué renvoyé dans une réponse de gestion de délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserId](userid.md) <br/> |Identifie le délégué. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[DelegatePermissions](delegatepermissions.md) <br/> |Contient les paramètres du niveau d’autorisation délégué. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ReceiveCopiesOfMeetingMessages](receivecopiesofmeetingmessages.md) <br/> |Indique si un délégué reçoit des copies des messages de réunion adressés au principal. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Indique si un délégué est autorisé à afficher des éléments de calendrier privés dans la boîte aux lettres du principal. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |Contient les identités des délégués à ajouter ou à mettre à jour dans une boîte aux lettres.  <br/> |
|[DelegateUserResponseMessageType](delegateuserresponsemessagetype.md) <br/> |Contient des messages de réponse pour les opérations de gestion des délégués. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md) 
- [Opération UpdateDelegate](updatedelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

