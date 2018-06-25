---
title: Nom (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: c719c55f-d625-4e64-846f-50ac91881443
description: L’élément Name représente le nom complet de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 6d30f06c3bfd77d2715798349ab084cdf81f21a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828505"
---
# <a name="name-emailaddress"></a>Nom (EmailAddress)

L’élément **Name** représente le nom complet de l’utilisateur de boîte aux lettres. 
  
```xml
<Name/>
```

**Chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Courrier électronique (EmailAddressType)](email-emailaddresstype.md) <br/> |Représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.  <br/> <br/>Vous trouverez ci-dessous le XPath pour cet élément :  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Boîte aux lettres (disponibilité)](mailbox-availability.md) <br/> | Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.  <br/><br/>  Les expressions XPath pour cet élément sont les suivantes :  <br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Cet élément peut se produire au maximum une seule fois dans l’élément de [courrier électronique (EmailAddressType)](email-emailaddresstype.md) . Cet élément n’est pas obligatoire. 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

