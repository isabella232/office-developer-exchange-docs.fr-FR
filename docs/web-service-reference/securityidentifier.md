---
title: SecurityIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: L’élément SecurityIdentifier représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité (SID).
ms.openlocfilehash: c55e4a7f7f0b8f8a40e6fcaf8d18e253a6da2679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468802"
---
# <a name="securityidentifier"></a>SecurityIdentifier

L’élément **SecurityIdentifier** représente la forme SDDL (Security Descriptor Definition Language) d’un identificateur de sécurité ( [sid](sid.md)).
  
```xml
<SecurityIdentifier/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |Représente un identificateur et un attribut de sécurité unique pour un groupe d’objets Active Directory dont le compte est membre.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[RestrictedGroupIdentifier](restrictedgroupidentifier.md) <br/> |Représente l’identificateur de sécurité de groupe et les attributs d’un groupe restreint au sein d’un jeton utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est utilisé dans l’en-tête SOAP (Simple Object Access Protocol).
  
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

