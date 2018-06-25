---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: L’élément MailboxType représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie.
ms.openlocfilehash: d7232377951e8d9c8f191ac856058bc28467cadd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828305"
---
# <a name="mailboxtype"></a>MailboxType

L’élément **MailboxType** représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie. 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

**MailboxTypeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse de messagerie entièrement résolu.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifie une liste de salles de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **MailboxType** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Boîte aux lettres  <br/> |Représente un objet Active Directory à extension messagerie.  <br/> |
|PublicDL  <br/> |Représente une liste de distribution publique.  <br/> |
|PrivateDL  <br/> |Représente une liste de distribution privée dans la boîte aux lettres d’un utilisateur.  <br/> |
|Contact  <br/> |Représente un contact dans la boîte aux lettres d’un utilisateur.  <br/> |
|Dossier public  <br/> |Représente un dossier public.  <br/> |
|Inconnu  <br/> |Représente un type inconnu de boîte aux lettres.  <br/> |
|OneOff  <br/> |Représente un membre unique d’une liste de distribution personnelle.  <br/> |
|GroupMailbox  <br/> |Représente une boîte aux lettres de groupe.  <br/> |
   
## <a name="remarks"></a>Remarques

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

