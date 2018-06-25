---
title: Entrée (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: L’élément d’entrée représente une adresse de messagerie unique pour un contact.
ms.openlocfilehash: 1852584e507c38da030815c37f85f7c4af4e2ba4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756192"
---
# <a name="entry-emailaddress"></a>Entrée (EmailAddress)

L’élément **d’entrée** représente une adresse de messagerie unique pour un contact. 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**EmailAddressDictionaryEntryType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Clé** <br/> | Identifie l’adresse de messagerie.<br/><br/>Les valeurs possibles de cet attribut sont les suivantes :<br/><br/>-EmailAddress1  <br/>-EmailAddress2  <br/>-EmailAddress3 <br/><br/>  Cet attribut est requis.  <br/> |
|**Name** <br/> |Définit le nom de l’utilisateur de boîte aux lettres. Cet attribut est facultatif.  <br/> |
|**RoutingType** <br/> |Définit le routage est utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet attribut est facultatif.  <br/> |
|**MailboxType** <br/> |Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[EmailAddresses](emailaddresses.md) <br/> |Représente une collection d'adresses de messagerie pour un contact.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

