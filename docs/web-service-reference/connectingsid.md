---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: L’élément ConnectingSID représente un compte à usurper lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation.
ms.openlocfilehash: 21cfcfc3590ea5a8b8ca5b53dfdb403e108e37f7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515970"
---
# <a name="connectingsid"></a>ConnectingSID

**L’élément ConnectingSID** représente un compte à usurper lorsque vous utilisez l’en-tête SOAP ExchangeImpersonation. 
  
- [ExchangeImpersonation](exchangeimpersonation.md) 
- [ConnectingSID](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

```xml
<ConnectingSID>
   <SmtpAddress/>
</ConnectingSID>
```

```xml
<ConnectingSID>
    <SID/> 
</ConnectingSID>
```

```xml
<ConnectingSID>
   <PrimarySmtpAddress/>
</ConnectingSID>
```

**ConnectingSIDType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |Représente le nom d’utilisateur principal (UPN) du compte à utiliser pour l’emprunt d’identité. Il doit s’y prendre à l’UPN pour le domaine dans lequel le compte d’utilisateur existe.  <br/> |
|[SID](sid.md) <br/> |Représente le formulaire SDDL (Security Descriptor Definition Language) de l’identificateur de sécurité (SID) du compte à utiliser pour l’emprunt d’identité.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Représente l’adresse SMTP (Simple Mail Transfer Protocol) principale du compte à utiliser pour Exchange’emprunt d’identité. Si l’adresse SMTP principale est fournie, une recherche supplémentaire du service d’annuaire Active Directory est nécessaire pour obtenir le SID de l’utilisateur. Nous vous recommandons d’utiliser le SID ou l’UPN s’ils sont disponibles.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Représente l’adresse SMTP (Simple Mail Transfer Protocol) du compte à utiliser pour l’Exchange de messagerie. Si l’adresse SMTP est fournie, une recherche Active Directory supplémentaire est nécessaire pour obtenir le SID de l’utilisateur. Nous vous recommandons d’utiliser le SID ou l’UPN s’ils sont disponibles.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Utilisé dans l’en-tête SOAP d’une requête. Lorsque cet élément est présent, l’appelant tente d’usurper l’identité du compte contenu dans **l’élément ExchangeImpersonation.**  <br/> Voici l’expression XPath de cet élément :  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Remarques

Le compte appelant doit avoir le droit d’emprunt d’identité **ms-exch sur** le serveur d’accès au client et le **droit ms-exch-MayImpersonate** sur la base de données de boîtes aux lettres qui contient la boîte aux lettres à usurper ou sur l’objet contact ou utilisateur Active Directory. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Autorisation de serveur à serveur dans EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

