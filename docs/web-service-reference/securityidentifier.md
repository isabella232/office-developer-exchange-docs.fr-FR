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
description: L’élément SecurityIdentifier représente le formulaire sécurité descripteur definition language (SDDL) d’un identificateur de sécurité (SID).
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829314"
---
# <a name="securityidentifier"></a>SecurityIdentifier

L’élément **SecurityIdentifier** représente le formulaire sécurité descripteur definition language (SDDL) d’un identificateur de sécurité ( [SID](sid.md)).
  
```xml
<SecurityIdentifier/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |Représente un identificateur de sécurité unique et un attribut pour un groupe d’objets Active Directory dont le compte est membre.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[RestrictedGroupIdentifier](restrictedgroupidentifier.md) <br/> |Représente l’identificateur du groupe de sécurité et les attributs d’un groupe restreint au sein d’un jeton utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est utilisé dans l’en-tête SOAP Simple Object Access Protocol ().
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

