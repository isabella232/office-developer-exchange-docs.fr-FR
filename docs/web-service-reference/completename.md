---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: L’élément CompleteName représente le nom complet d’un contact.
ms.openlocfilehash: 873d372657089d21e86025cdf7812659ac505491
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543554"
---
# <a name="completename"></a>CompleteName

**L’élément CompleteName** représente le nom complet d’un contact. 
  
```xml
<CompleteName>
   <Title/>
   <FirstName/>
   <MiddleName/>
   <LastName/>
   <Suffix/>
   <Initials/>
   <FullName/>
   <Nickname/>
   <YomiFirstName/>
   <YomiLastName/>
</CompleteName>
```

 **CompleteNameType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Title](title.md) <br/> |Représente le titre d’un contact.  <br/> |
|[FirstName](firstname.md) <br/> |Représente le prénom du contact.  <br/> |
|[MiddleName](middlename.md) <br/> |Représente le deuxième prénom d'un contact.  <br/> |
|[LastName](lastname.md) <br/> |Représente le nom de famille d’un contact.  <br/> |
|[Suffix](suffix.md) <br/> |Représente un suffixe du nom d’un contact.  <br/> |
|[Initials](initials.md) <br/> |Représente les initiales d'un contact.  <br/> |
|[FullName](fullname.md) <br/> |Représente le nom complet d’un contact.  <br/> |
|[Nickname](nickname.md) <br/> |Représente le surnom d'un contact.  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |Représente le nom utilisé au Japon pour l’orthographe phonétique ou de recherche d’un prénom japonais.  <br/> |
|[YomiLastName](yomilastname.md) <br/> |Représente le nom utilisé au Japon pour l’orthographe phonétique ou de recherche d’un nom japonais.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

La propriété CompleteName fait partie de la [forme Par](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) défaut. Dans la version initiale de Microsoft Exchange Server 2007, la propriété CompleteName est renvoyée par l’opération [GetItem,](getitem-operation.md)mais pas par [l’opération FindItem](finditem-operation.md). À partir Exchange Server 2007 Service Pack 1 (SP1), l’opération [FindItem](finditem-operation.md) renvoie également la propriété CompleteName avec la forme [Default.](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) Cette modification n’affecte pas le schéma. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Creating Contacts (Exchange Web Services)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

