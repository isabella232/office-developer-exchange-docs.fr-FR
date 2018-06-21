---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: L’élément AlternateMailbox représente une autre boîte aux lettres.
ms.openlocfilehash: 8eb53e4846ad55916e2c5876606c00c0f2e371ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19755251"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

L’élément **AlternateMailbox** représente une autre boîte aux lettres. 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 **AlternateMailbox**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (SOAP)](type-soap.md) <br/> |Représente le type de boîte aux lettres de substitution.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Représente le nom complet de boîte aux lettres de substitution.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Représente le nom unique hérité autre boîte aux lettres.  <br/> |
|[Serveur (SOAP)](server-soap.md) <br/> |Représente le serveur de boîtes aux lettres de substitution.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Représente la boîte aux lettres autre adresse SMTP.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Représente une collection d’autres boîtes aux lettres.  <br/> |
   
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

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

