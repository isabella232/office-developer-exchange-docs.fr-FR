---
title: InvalidRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: L’élément InvalidRecipient contient l’adresse SMTP du destinataire non valide et des informations sur la raison pour laquelle il n’est pas valide.
ms.openlocfilehash: 507cdf23d42477e7b70258b674246463e10f975b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539534"
---
# <a name="invalidrecipient"></a>InvalidRecipient

**L’élément InvalidRecipient contient** l’adresse SMTP du destinataire non valide et des informations sur la raison pour laquelle il n’est pas valide. 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 **InvalidRecipientType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Contient l’adresse SMTP du destinataire non valide. Cet élément est obligatoire.  <br/> |
|[ResponseCode (InvalidRecipientResponseCodeType)](responsecode-invalidrecipientresponsecodetype.md) <br/> |Fournit un code d’erreur qui identifie l’erreur spécifique rencontrée par la demande. Cet élément est obligatoire.  <br/> |
|[MessageText](messagetext.md) <br/> |Fournit une description textuelle de l’état de la réponse. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[InvalidRecipients](invalidrecipients.md) <br/> |Représente les destinataires d’une demande de partage de dossier qui ne sont pas valides.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetSharingMetadata](getsharingmetadata-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

