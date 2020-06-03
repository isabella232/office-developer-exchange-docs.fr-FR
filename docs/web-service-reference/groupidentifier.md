---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: L’élément GroupIdentifier représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets de service d’annuaire Active Directory dont le compte est membre.
ms.openlocfilehash: 8b427b9228cc5e66f46f70389acf2fa4bcd283b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530802"
---
# <a name="groupidentifier"></a>GroupIdentifier

L’élément **GroupIdentifier** représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets de service d’annuaire Active Directory dont le compte est membre. 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 **SidAndAttributesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Attributs** <br/> |Contient les attributs de groupe.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |Représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité ([sid](sid.md)) qui représente le groupe.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupSids](groupsids.md) <br/> |Représente une collection d’identificateurs de sécurité d’objets de groupe Active Directory qui constituent un jeton de compte pour la sérialisation de jetons. La sérialisation de jetons n’est pas prise en charge.  <br/> |
   
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

