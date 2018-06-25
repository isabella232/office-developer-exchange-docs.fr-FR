---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: L’élément EnhancedLocation spécifie les informations d’emplacement telles que le nom, adresse et notes facultatives sur un emplacement.
ms.openlocfilehash: 90397cfc622fed40c561d30c13d6617eb979a68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756187"
---
# <a name="enhancedlocation"></a>EnhancedLocation

L’élément **EnhancedLocation** spécifie les informations d’emplacement telles que le nom, adresse et notes facultatives sur un emplacement. 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 **EnhancedLocationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom complet d’un dossier, contact, liste de distribution, délégué utilisateur, emplacement ou règle.  <br/> |
|[Annotation](annotation.md) <br/> |Contient des notes facultatives ajoutés par un utilisateur.  <br/> |
|[PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |Spécifie l’adresse postale pour un personnage.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
   
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

