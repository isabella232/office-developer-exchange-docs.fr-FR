---
title: Entrée (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: b028c5c7-3494-4ecd-96d1-78783daa660f
description: L’élément Entry représente une adresse de messagerie unique pour un contact.
ms.openlocfilehash: 96351a82e113f2c4aa73776e89e1eb7e7a683433
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520667"
---
# <a name="entry-emailaddress"></a>Entrée (EmailAddress)

**L’élément Entry** représente une adresse de messagerie unique pour un contact. 
  
```XML
<Entry Key="" Name="" RoutingType="" MailboxType="" />
```

**EmailAddressDictionaryEntryType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Clé** <br/> | Identifie l’adresse de messagerie.<br/><br/>Les valeurs possibles pour cet attribut sont les suivantes :<br/><br/>- EmailAddress1  <br/>- EmailAddress2  <br/>- EmailAddress3 <br/><br/>  Cet attribut est obligatoire.  <br/> |
|**Name** <br/> |Définit le nom de l’utilisateur de la boîte aux lettres. Cet attribut est facultatif.  <br/> |
|**RoutingType** <br/> |Définit le routage utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet attribut est facultatif.  <br/> |
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

