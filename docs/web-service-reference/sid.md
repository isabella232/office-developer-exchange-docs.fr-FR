---
title: SID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SID
api_type:
- schema
ms.assetid: 2f33b29b-163b-4106-a74d-6fb76ec38951
description: L’élément SID représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID) pour le compte à utiliser pour l’emprunt d’identité ou l’accès délégué.
ms.openlocfilehash: efcea42c12ec1d26ea31fdb8de337c37a2338a96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829492"
---
# <a name="sid"></a>SID

L’élément **SID** représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID) pour le compte à utiliser pour l’emprunt d’identité ou l’accès délégué. 
  
```xml
<SID/>
```

 **SIDType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Représente un compte pour emprunter l’identité lors de l’utilisation de l’en-tête SOAP ExchangeImpersonation.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[Nom d’utilisateur](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur disposant des autorisations d’accès au dossier.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est une représentation de chaîne d’un identificateur de sécurité.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

