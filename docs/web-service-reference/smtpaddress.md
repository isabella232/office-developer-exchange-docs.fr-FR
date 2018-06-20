---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: L’élément SmtpAddress représente l’adresse SMTP Simple Mail Transfer Protocol () d’un compte à utiliser pour l’emprunt d’identité ou une adresse de destinataire SMTP Simple Mail Transfer Protocol () d’un calendrier ou d’une demande de partage de contact.
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829511"
---
# <a name="smtpaddress"></a>SmtpAddress

L’élément **SmtpAddress** représente l’adresse SMTP Simple Mail Transfer Protocol () d’un compte à utiliser pour l’emprunt d’identité ou une adresse de destinataire SMTP Simple Mail Transfer Protocol () d’un calendrier ou d’une demande de partage de contact. 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Représente un destinataire non valide pour un partage de calendrier ou un message de partage de contact.  <br/> |
|[Destinataires (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Représente une collection de destinataires qui auront accès au dossier partagé.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

