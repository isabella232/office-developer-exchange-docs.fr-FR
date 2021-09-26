---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: L’élément ResponseCode fournit des informations sur la raison pour laquelle le destinataire n’est pas valide.
ms.openlocfilehash: 33cd05aca672e250f288aec72d876734132d2e36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544807"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a>ResponseCode (InvalidRecipientResponseCodeType)

**L’élément ResponseCode** fournit des informations sur la raison pour laquelle le destinataire n’est pas valide. 
  
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

Le tableau suivant répertorie les valeurs possibles pour **l’élément ResponseCode.** 
  
|**Code**|**Description**|
|:-----|:-----|
|OtherError  <br/> |Indique que l’erreur n’est pas spécifiée par un autre code de réponse d’erreur.  <br/> |
|RecipientOrganizationNotFederated  <br/> |Indique qu’une relation de partage n’est pas disponible avec l’organisation spécifiée dans l’adresse de messagerie SMTP du destinataire.  <br/> |
|CannotObtainTokenFromSTS  <br/> |Indique qu’il y a eu un problème lors de l’obtention d’un jeton de sécurité à partir du serveur de jetons.  <br/> |
|SystemPolicyBlocksSharingWithThisRecipient  <br/> |Indique que l’administrateur système a définie une stratégie système qui bloque le partage avec le destinataire spécifié.  <br/> |
|RecipientOrganizationFederatedWithUnknownTokenIssuer  <br/> |Indique que le service de jeton sécurisé utilisé par le destinataire spécifié est inconnu.  <br/> |
   
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

