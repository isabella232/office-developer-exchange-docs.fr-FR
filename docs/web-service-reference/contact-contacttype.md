---
title: Contact (TypeContact)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f7119b7-f5b4-484d-a7de-fa74836d9aee
description: L’élément de Contact spécifie un contact dans le magasin de contacts unifié.
ms.openlocfilehash: f1593da78a46851c7db43abc567eb66c0c74e0f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755552"
---
# <a name="contact-contacttype"></a>Contact (TypeContact)

L’élément de **Contact** spécifie un contact dans le magasin de contacts unifié. 
  
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

 **TypeContact**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[PersonName](personname.md) <br/> |Spécifie le nom d’un participant.  <br/> |
|[BusinessName](businessname.md) <br/> |Spécifie le nom de l’entreprise.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Représente une collection de numéros de téléphone pour un contact.  <br/> |
|[URL](urls.md) <br/> |Spécifie un tableau d’URL pour un personnage.  <br/> |
|[EmailAddresses (ArrayOfExtractedEmailAddresses)](emailaddresses-arrayofextractedemailaddresses.md) <br/> |Spécifie un tableau des adresses de messagerie extraits.  <br/> |
|[Adresses (ArrayOfAddressesType)](addresses-arrayofaddressestype.md) <br/> |Spécifie un tableau des éléments de **l’adresse** .  <br/> |
|[ContactString](contactstring.md) <br/> |Spécifie le nom complet d’un contact.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Contacts (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Spécifie un tableau des contacts.  <br/> |
   
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

