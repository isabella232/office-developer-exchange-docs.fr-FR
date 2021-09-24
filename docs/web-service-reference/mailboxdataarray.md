---
title: MailboxDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxDataArray
api_type:
- schema
ms.assetid: a14af788-beee-452c-b5d0-37bcb4ef02ff
description: L’élément MailboxDataArray contient une liste de boîtes aux lettres à interroger pour obtenir des informations de disponibilité.
ms.openlocfilehash: e6bd5bcffa776bb284d22a76d785637a7015adac
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540774"
---
# <a name="mailboxdataarray"></a>MailboxDataArray

**L’élément MailboxDataArray contient** une liste de boîtes aux lettres à interroger pour obtenir des informations de disponibilité. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
- [MailboxDataArray](mailboxdataarray.md)
  
- [MailboxData](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

**ArrayOfMailboxData**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Représente un utilisateur de boîte aux lettres individuel et des options pour le type de données à retourner sur l’utilisateur de la boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur. Il s’agit d’un élément racine.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft® Exchange Server 2007 où le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

