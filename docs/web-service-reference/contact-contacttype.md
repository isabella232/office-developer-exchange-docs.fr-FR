---
title: Contact (ContactType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: L’élément Contact spécifie un contact dans le magasin de contacts unifié.
ms.openlocfilehash: e52573841f934a11c05a1da9e19f91146ed9c774
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511992"
---
# <a name="contact-contacttype"></a>Contact (ContactType)

**L’élément Contact** spécifie un contact dans le magasin de contacts unifié. 
  
```XML
<Contact>
    <PersonName></PersonName>
    <BusinessName></BusinessName>
    <PhoneNumbers></PhoneNumbers>
    <Urls></Urls>
    <EmailAddresses></EmailAddresses>
    <Addresses></Addesses>    <ContactString></ContactString
</Contact>
```

 **ContactType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[PersonName](personname.md) <br/> |Spécifie le nom d’un individu.  <br/> |
|[BusinessName](businessname.md) <br/> |Spécifie le nom d’une entreprise.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Représente une collection de numéros de téléphone pour un contact.  <br/> |
|[URL](urls.md) <br/> |Spécifie un tableau d’URL pour un personnage.  <br/> |
|[EmailAddresses (ArrayOfExtractedEmailAddresses)](emailaddresses-arrayofextractedemailaddresses.md) <br/> |Spécifie un tableau d’adresses de messagerie extraites.  <br/> |
|[Addresses (ArrayOfAddressesType)](addresses-arrayofaddressestype.md) <br/> |Spécifie un tableau d’éléments **Address.**  <br/> |
|[ContactString](contactstring.md) <br/> |Spécifie le nom complet d’un contact.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Contacts (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Spécifie un tableau de contacts.  <br/> |
   
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

