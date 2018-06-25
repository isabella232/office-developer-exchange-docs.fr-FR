---
title: DelegateUsers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUsers
api_type:
- schema
ms.assetid: f30f80d9-20c8-41cc-afc7-a5eec1e0c5ea
description: L’élément DelegateUsers contient les identités de délégués à ajouter ou mettre à jour dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a078707ae6b1676ca5a32ba718add93debd498fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755836"
---
# <a name="delegateusers"></a>DelegateUsers

L’élément **DelegateUsers** contient les identités de délégués à ajouter ou mettre à jour dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

**ArrayOfDelegateUserType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateur_délégué](delegateuser.md) <br/> |Identifie un délégué unique à ajouter ou mettre à jour dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Définit une demande pour ajouter des délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Définit une demande de mise à jour des délégués dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
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
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

