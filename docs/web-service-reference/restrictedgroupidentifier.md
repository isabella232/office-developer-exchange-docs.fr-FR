---
title: RestrictedGroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RestrictedGroupIdentifier
api_type:
- schema
ms.assetid: a3ea3c81-9f99-4836-8cb4-2384ea63f093
description: L’élément RestrictGroupIdentifier représente l’identificateur de sécurité de groupe (SID) et les attributs d’un groupe restreint dans un jeton d’utilisateur.
ms.openlocfilehash: 65b356f4a8195979d751a3f5288940b391f51939
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544779"
---
# <a name="restrictedgroupidentifier"></a>RestrictedGroupIdentifier

**L’élément RestrictGroupIdentifier** représente l’identificateur de sécurité de groupe (SID) et les attributs d’un groupe restreint dans un jeton d’utilisateur. 
  
```xml
<RestrictedGroupIdentifier Attributes="">
   <SecurityIdentifier/>
</RestrictedGroupIdentifier>
```

 **SidAndAttributesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Attributs** <br/> |Contient des attributs de groupe.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |Représente le formulaire SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Représente une collection de groupes restreints dans un jeton d’utilisateur. La sérialisation des jetons n’est pas prise en charge.  <br/> |
   
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

