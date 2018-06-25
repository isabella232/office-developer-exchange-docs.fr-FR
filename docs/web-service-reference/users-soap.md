---
title: Utilisateurs (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: L’élément utilisateurs représente une collection d’adresses de messagerie des utilisateurs pour lesquels les paramètres doivent être récupérés.
ms.openlocfilehash: d7655f0020a315dcb32adbbc58610ca0e630c1fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838976"
---
# <a name="users-soap"></a>Utilisateurs (SOAP)

L’élément **utilisateurs** représente une collection d’adresses de messagerie des utilisateurs pour lesquels les paramètres doivent être récupérés. 
  
```XML
<Users>
   <User/>
</Users>
```

 **Utilisateurs**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateur (SOAP)](user-soap.md) <br/> |Représente l’adresse de messagerie d’un utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Représente une demande pour récupérer les paramètres spécifiés pour un ou plusieurs utilisateurs.  <br/> |
|[Demande (SOAP)](request-soap.md) <br/> |Contient les paramètres de configuration requise et les utilisateurs cibles.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)

