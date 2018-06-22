---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: L’élément EntityExtractionResult spécifie la propriété EntityExtractionResult d’un élément.
ms.openlocfilehash: ef99629beb95f1e1123569fa99e3f495c1b56e95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756197"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

L’élément **EntityExtractionResult** spécifie la propriété **EntityExtractionResult** d’un élément. 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 **EntityExtractionResultType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Adresses (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |Spécifie un tableau d’éléments **AddressEntity** .  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |Spécifie un tableau d’éléments **MeetingSuggestion** .  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |Spécifie un tableau d’éléments **TaskSuggestion** .  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |Spécifie un tableau des entités d’adresse de messagerie.  <br/> |
|[Contacts (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Spécifie un tableau des contacts.  <br/> |
|[URL (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |Spécifie un tableau d’URL.  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |Spécifie un tableau des numéros de téléphone.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Item](item.md) <br/> |Représente un élément générique dans la banque d’informations Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

