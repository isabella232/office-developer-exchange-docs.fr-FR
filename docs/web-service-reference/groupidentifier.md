---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: L’élément GroupIdentifier représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets de service d’annuaire Active Directory dont le compte est membre.
ms.openlocfilehash: c96d0ca673d9b488266f08abbbd6546aaeb9f5a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533158"
---
# <a name="groupidentifier"></a>GroupIdentifier

**L’élément GroupIdentifier** représente un identificateur de sécurité et un attribut uniques pour un groupe d’objets de service d’annuaire Active Directory dont le compte est membre. 
  
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
|**Attributs** <br/> |Contient des attributs de groupe.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |Représente le formulaire SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité[(SID)](sid.md)qui représente le groupe.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupSids](groupsids.md) <br/> |Représente une collection d’identificateurs de sécurité d’objets de groupe Active Directory qui constituent un jeton de compte pour la sérialisation des jetons. La sérialisation des jetons n’est pas prise en charge.  <br/> |
   
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

