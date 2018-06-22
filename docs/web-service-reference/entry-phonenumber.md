---
title: Entrée (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: L’élément d’entrée représente un numéro de téléphone d’un contact.
ms.openlocfilehash: 3953488fb0b57fcf01c2fb99039478bbe03c7f5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756201"
---
# <a name="entry-phonenumber"></a>Entrée (PhoneNumber)

L’élément **d’entrée** représente un numéro de téléphone d’un contact. 
  
```xml
<Entry Key=""/>
```

 **PhoneNumberDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Clé** <br/> | Identifie le numéro de téléphone. L’attribut Key est de type **PhoneNumberKeyType**.<br/><br/> Les valeurs possibles de cet attribut sont les suivantes :<br/><br/>-AssistantPhone  <br/>-BusinessFax  <br/>-BusinessPhone  <br/>-BusinessPhone2  <br/>-Rappel  <br/>-Téléphone de voiture  <br/>-CompanyMainPhone  <br/>-Télécopie personnelle  <br/>-HomePhone  <br/>-HomePhone2  <br/>-RNIS  <br/>-MobilePhone  <br/>-OtherFax  <br/>-OtherTelephone  <br/>-Récepteur de radiomessagerie  <br/>-PrimaryPhone  <br/>-RadioPhone  <br/>-Télex  <br/>-TtyTddPhone  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |Représente une collection de numéros de téléphone pour un contact.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente un numéro de téléphone est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Note

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Creating Contacts (Exchange Web Services)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [Updating Contacts](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Deleting Contacts](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

