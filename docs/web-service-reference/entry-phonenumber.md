---
title: Entrée (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: L’élément Entry représente un numéro de téléphone pour un contact.
ms.openlocfilehash: f9f8f08c8d167614bfc5772d6d74ebee77234c70
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545243"
---
# <a name="entry-phonenumber"></a>Entrée (PhoneNumber)

**L’élément Entry** représente un numéro de téléphone pour un contact. 
  
```xml
<Entry Key=""/>
```

 **PhoneNumberDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Clé** <br/> | Identifie le numéro de téléphone. L’attribut Key est de type **PhoneNumberKeyType**.<br/><br/> Les valeurs possibles pour cet attribut sont les suivantes :<br/><br/>- AssistantPhone  <br/>- BusinessFax  <br/>- BusinessPhone  <br/>- BusinessPhone2  <br/>- Rappel  <br/>- CarPhone  <br/>- CompanyMainPhone  <br/>- HomeFax  <br/>- HomePhone  <br/>- HomePhone2  <br/>- Isdn  <br/>- MobilePhone  <br/>- OtherFax  <br/>- OtherTelephone  <br/>- Pager  <br/>- PrimaryPhone  <br/>- RadioPhone  <br/>- Telex  <br/>- TtyTddPhone  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |Représente une collection de numéros de téléphone pour un contact.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur texte qui représente un numéro de téléphone est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Création de Contacts (Services Web Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [Updating Contacts](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Deleting Contacts](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

