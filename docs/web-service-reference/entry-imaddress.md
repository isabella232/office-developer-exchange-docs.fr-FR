---
title: Entrée (IMAddress)
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
ms.assetid: ee444170-7353-4e86-86c6-d7300a2f1777
description: L’élément Entry représente une adresse de messagerie instantanée (IM) pour un contact.
ms.openlocfilehash: b6cc37447eb0f231e9e852a6c3cd64d6e1f3a89f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460700"
---
# <a name="entry-imaddress"></a>Entrée (IMAddress)

L’élément **entry** représente une adresse de messagerie instantanée (im) pour un contact. 
  
```xml
<Entry Key=""/>
```

 **ImAddressDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Key** <br/> | Identifie l’adresse de messagerie instantanée.<br/><br/>Les valeurs possibles pour cet attribut sont les suivantes :<br/><br/>- ImAddress1  <br/>- ImAddress2  <br/>- ImAddress3  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ImAddresses](imaddresses.md) <br/> |Représente une collection d’adresses de messagerie instantanée pour un contact.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente l’adresse de messagerie instantanée est requise si cet élément est utilisé.
  
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

