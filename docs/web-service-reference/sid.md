---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: L’élément SID représente le formulaire SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID) du compte à utiliser pour l’emprunt d’identité ou l’accès délégué.
ms.openlocfilehash: 436f284b59d5146b481a25b7b0986db4aeee67ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547056"
---
# <a name="sid"></a>SID

L’élément **SID** représente le formulaire SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID) du compte à utiliser pour l’emprunt d’identité ou l’accès délégué. 
  
```xml
<SID/>
```

 **SIDType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Représente un compte à usurper lors de l’utilisation de l’en-tête SOAP ExchangeImpersonation.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[UserId](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur ayant des autorisations d’accès aux dossiers.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est une représentation sous la chaîne d’un SID.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

