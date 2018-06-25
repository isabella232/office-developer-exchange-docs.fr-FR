---
title: Utilisateur (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: L’élément représente l’identité d’un utilisateur unique.
ms.openlocfilehash: a8dcb22f5c74a9622f978f34e48146115351fe82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838947"
---
# <a name="user-soap"></a>Utilisateur (SOAP)

**L’élément** représente l’identité d’un utilisateur unique. 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 **User**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Représente le nom unique hérité autre boîte aux lettres.  <br/> |
|[Boîte aux lettres (SOAP)](mailbox-soap.md) <br/> |Contient l’adresse de messagerie de l’utilisateur à être découvert.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration demandé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateurs (SOAP)](users-soap.md) <br/> |Représente une collection d’éléments de **l’utilisateur** .  <br/> |
   
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
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

