---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: L’élément ConnectingSID représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.
ms.openlocfilehash: 6e0bb90e197ce22bcd982a6d51954a88f3a2cf03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755546"
---
# <a name="connectingsid"></a>ConnectingSID

L’élément **ConnectingSID** représente un compte pour emprunter l’identité lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation. 
  
[ExchangeImpersonation](exchangeimpersonation.md)
  
[ConnectingSID](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

 **ConnectingSIDType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Au PrincipalName](principalname.md) <br/> |Représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité. Il doit s’agir de l’UPN pour le domaine où le compte d’utilisateur existe.  <br/> |
|[SID](sid.md) <br/> |Représente le formulaire sécurité descripteur definition language (SDDL) de l’identificateur de sécurité (SID) pour le compte à utiliser pour l’emprunt d’identité.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Représente l’adresse SMTP Simple Mail Transfer Protocol () principal du compte à utiliser pour l’emprunt d’identité Exchange. Si l’adresse SMTP principale est fourni, une recherche de service d’annuaire Active Directory supplémentaire seront coût afin d’obtenir le SID de l’utilisateur. Nous vous recommandons d’utiliser le SID ou UPN si elles sont disponibles.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Représente l’adresse SMTP Simple Mail Transfer Protocol () du compte à utiliser pour l’emprunt d’identité Exchange. Si l’adresse SMTP est fourni, une recherche Active Directory supplémentaire seront coût afin d’obtenir le SID de l’utilisateur. Nous vous recommandons d’utiliser le SID ou UPN si elles sont disponibles.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Utilisé dans l’en-tête SOAP d’une demande. Lorsque cet élément est présent, l’appelant essaie d’emprunter l’identité du compte qui est contenu dans l’élément **ExchangeImpersonation** .  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Remarques

Le compte d’appel doit avoir **ms-exch-l’emprunt d’identité** sur le serveur d’accès au Client et le **ms-exch-MayImpersonate** droite sur soit la base de données de boîtes aux lettres contenant la boîte aux lettres pour emprunter l’identité ou l’utilisateur Active Directory ou un contact objet. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Autorisation de serveur à serveur dans EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

