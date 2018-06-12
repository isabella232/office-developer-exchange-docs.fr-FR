---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: L’élément ResponseCode fournit des informations sur la raison pour laquelle le destinataire n’est pas valide.
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

L’élément **ResponseCode** fournit des informations sur la raison pour laquelle le destinataire n’est pas valide. 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |Contient l'adresse SMTP du destinataire non valide et plus d'informations sur la raison pour laquelle le destinataire n'est pas valide.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **ResponseCode** . 
  
|**Code**|**Description**|
|:-----|:-----|
|OtherError  <br/> |Indique que l’erreur n’est pas spécifié par un autre code d’erreur.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Indique qu’une relation de partage n’est pas disponible avec l’organisation spécifiée dans l’adresse de messagerie SMTP du destinataire.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Indique qu’il y a un problème d’obtention d’un jeton de sécurité à partir du serveur d’émission de jeton.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Indique que l’administrateur système a défini une stratégie système qui bloque le partage avec le destinataire spécifié.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Indique que le service de jeton de sécurité utilisé par le destinataire spécifié est inconnu.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetSharingMetadata](getsharingmetadata-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

