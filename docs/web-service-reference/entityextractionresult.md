---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: L’élément EntityExtractionResult spécifie la propriété EntityExtractionResult d’un élément.
ms.openlocfilehash: b550953233999bfd9c4dc08a7f892e798029df3c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520674"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

**L’élément EntityExtractionResult** spécifie la propriété **EntityExtractionResult** d’un élément. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Addresses (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |Spécifie un tableau d’éléments **AddressEntity.**  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |Spécifie un tableau **d’éléments MeetingSuggestion.**  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |Spécifie un tableau **d’éléments TaskSuggestion.**  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |Spécifie un tableau d’entités d’adresse de messagerie.  <br/> |
|[Contacts (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Spécifie un tableau de contacts.  <br/> |
|[URL (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |Spécifie un tableau d’URL.  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |Spécifie un tableau de numéros de téléphone.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Item](item.md) <br/> |Représente un élément générique dans le magasin Exchange de données.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

