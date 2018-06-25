---
title: Courrier électronique (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Email
api_type:
- schema
ms.assetid: dfffa1d5-2c3c-4f56-af63-5853df462e58
description: L’élément de courrier électronique représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability.
ms.openlocfilehash: 0e7848d7c4f5001ed86b06d11af1d7623b4bf1f0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756095"
---
# <a name="email-emailaddresstype"></a>Courrier électronique (EmailAddressType)

L’élément de **courrier électronique** représente l’utilisateur de boîte aux lettres pour une requête GetUserAvailability. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)  
- [MailboxDataArray](mailboxdataarray.md) 
- [MailboxData](mailboxdata.md) 
- [Courrier électronique (EmailAddressType)](email-emailaddresstype.md)
  
```xml
<Email>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Email>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom (EmailAddress)](name-emailaddress.md) <br/> |Représente le nom complet de l’utilisateur de boîte aux lettres.  <br/> |
|[Adresse (chaîne)](address-string.md) <br/> |Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Représente le protocole de routage pour le message.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxData](mailboxdata.md) <br/> |Représente un utilisateur de boîte aux lettres et les options pour le type de données à renvoyer sur l’utilisateur de boîte aux lettres.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.
  
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

