---
title: UserSid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: L’élément UserSid représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité utilisateur dans un en-tête SOAP de contexte de sécurité sérialisé. La sérialisation des jetons n’est pas prise en charge.
ms.openlocfilehash: b32c9fc8347fba07bff57b942adf6510d37ebf2f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517349"
---
# <a name="usersid"></a>UserSid

**L’élément UserSid** représente la forme SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité utilisateur dans un en-tête SOAP de contexte de sécurité sérialisé. La sérialisation des jetons n’est pas prise en charge. 
  
```xml
<UserSid/>
```

 **String**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Utilisé dans l’en-tête SOAP pour la sérialisation des jetons dans l’authentification de serveur à serveur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’identificateur de sécurité d’un utilisateur.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

