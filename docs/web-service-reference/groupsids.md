---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: L’élément GroupSids représente une collection d’identificateurs de sécurité d’objet de groupe de service d’annuaire Active Directory.
ms.openlocfilehash: 9dde1c87a82dbef2a9e1278de2cc202189f309c7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539674"
---
# <a name="groupsids"></a>GroupSids

**L’élément GroupSids** représente une collection d’identificateurs de sécurité d’objet de groupe de service d’annuaire Active Directory. 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 **NonEmptyArrayOfGroupIdentifiersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |Représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets Active Directory dont le compte est membre.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Utilisé dans l’en-tête SOAP (Simple Object Access Protocol) pour la sérialisation des jetons dans l’authentification de serveur à serveur. La sérialisation des jetons n’est pas prise en charge.  <br/> |
   
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

