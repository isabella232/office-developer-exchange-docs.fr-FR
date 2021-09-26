---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: L’élément AlternateMailbox représente une autre boîte aux lettres.
ms.openlocfilehash: 3646efef9b63b2af8dbba41a07a86462e18ac1c1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543722"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

**L’élément AlternateMailbox** représente une autre boîte aux lettres. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (SOAP)](type-soap.md) <br/> |Représente le type de boîte aux lettres de remplacement.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Représente le nom complet de la boîte aux lettres de remplacement.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Représente l’autre nom d’héritage de boîte aux lettres.  <br/> |
|[Server (SOAP)](server-soap.md) <br/> |Représente l’autre serveur de boîtes aux lettres.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Représente l’adresse SMTP de la boîte aux lettres de remplacement.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Représente une collection de boîtes aux lettres de remplacement.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

