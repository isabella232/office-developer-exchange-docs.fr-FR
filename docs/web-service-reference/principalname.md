---
title: Au PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: L’élément au PrincipalName représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité Exchange.
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828882"
---
# <a name="principalname"></a>Au PrincipalName

L’élément **au PrincipalName** représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité Exchange. 
  
```xml
<PrincipalName/>
```

 **PrincipalNameType**
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
   
## <a name="text-value"></a>Valeur de texte

La valeur de text représente l’UPN d’un utilisateur. Cette valeur existe sur l’objet utilisateur dans le service d’annuaire Active Directory. Contient le nom d’utilisateur et un nom de domaine qui identifie le domaine dans lequel le compte d’utilisateur se trouve, dans le format suivant : `someone@example.com`.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Autorisation de serveur à serveur dans EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

