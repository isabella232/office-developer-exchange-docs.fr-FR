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
description: L’élément AlternateMailbox représente une boîte aux lettres de substitution.
ms.openlocfilehash: 9019f85a373cc186cc9dadddceee3dc9d11b3854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466156"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

L’élément **AlternateMailbox** représente une boîte aux lettres de substitution. 
  
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
|[Type (SOAP)](type-soap.md) <br/> |Représente le type de boîte aux lettres de substitution.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Représente le nom d’affichage de la boîte aux lettres de remplacement.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Représente le nom unique hérité de la boîte aux lettres de substitution.  <br/> |
|[Serveur (SOAP)](server-soap.md) <br/> |Représente le serveur de boîtes aux lettres de substitution.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Représente l’adresse SMTP de la boîte aux lettres de substitution.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Représente une collection de boîtes aux lettres de substitution.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

