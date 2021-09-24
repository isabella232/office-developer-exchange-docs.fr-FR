---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: L’élément SmtpAddress représente l’adresse SMTP (Simple Mail Transfer Protocol) d’un compte à utiliser pour l’emprunt d’identité ou une adresse de destinataire SMTP (Simple Mail Transfer Protocol) d’une demande de partage de calendrier ou de contact.
ms.openlocfilehash: c10e18ce77a1002a9c7a94718e8e9a2bd3877d8d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539086"
---
# <a name="smtpaddress"></a>SmtpAddress

L’élément **SmtpAddress** représente l’adresse SMTP (Simple Mail Transfer Protocol) d’un compte à utiliser pour l’emprunt d’identité ou une adresse de destinataire SMTP (Simple Mail Transfer Protocol) d’une demande de partage de calendrier ou de contact. 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Représente un compte à usurper lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Représente un destinataire non valide pour un message de partage de calendrier ou de contact.  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Représente une collection de destinataires qui auront accès au dossier partagé.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Définit une demande d’obtenir l’identificateur de dossier local d’un dossier partagé spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

