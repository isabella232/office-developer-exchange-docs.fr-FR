---
title: Boîte aux lettres (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4ad59e5b-4047-4c34-a318-ca06c31d3de8
description: L’élément de boîte aux lettres contient l’adresse de messagerie de l’utilisateur à être découvert.
ms.openlocfilehash: b98397dadf8c467031eb8febe9732d4e426372e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828253"
---
# <a name="mailbox-soap"></a>Boîte aux lettres (SOAP)

L’élément de **boîte aux lettres** contient l’adresse de messagerie de l’utilisateur à être découvert. 
  
```XML
<Mailbox/>
```

**string**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateur (SOAP)](user-soap.md) <br/> |Représente l’identité d’un utilisateur unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément de **boîte aux lettres** est l’adresse de messagerie de l’utilisateur à être découvert. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)

