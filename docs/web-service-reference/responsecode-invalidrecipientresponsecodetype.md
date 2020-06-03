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
ms.openlocfilehash: d78de64de7725007ec51a55dad13d1cc892a25e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529720"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

L’élément **ResponseCode** fournit des informations sur la raison pour laquelle le destinataire n’est pas valide. 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 **InvalidRecipientResponseCodeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[InvalidRecipient](invalidrecipient.md) <br/> |Contient l'adresse SMTP du destinataire non valide et plus d'informations sur la raison pour laquelle le destinataire n'est pas valide.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **ResponseCode** . 
  
|**Code**|**Description**|
|:-----|:-----|
|OtherError  <br/> |Indique que l’erreur n’est pas spécifiée par un autre code de réponse d’erreur.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Indique qu’une relation de partage n’est pas disponible pour l’organisation spécifiée dans l’adresse de messagerie SMTP du destinataire.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Indique qu’un problème est survenu lors de l’obtention d’un jeton de sécurité à partir du serveur de jetons.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Indique que l’administrateur système a défini une stratégie système qui bloque le partage avec le destinataire spécifié.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Indique que le service d’émission de jeton de sécurité utilisé par le destinataire spécifié est inconnu.  <br/> |
   
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

