---
title: Compte (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: L’élément Account spécifie les paramètres de compte de l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462317"
---
# <a name="account-pox"></a>Compte (POX)

L’élément **Account** spécifie les paramètres de compte de l’utilisateur ou contient des réponses d’erreur. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
- [Réponse (POX)](response-pox.md)
- [Compte (POX)](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Représente le type de compte.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Fournit des informations qui permettent de déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration de l’utilisateur.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Contient une valeur qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Contient l’URL de l’ordinateur qui exécute Exchange Server sur lequel le rôle serveur d’accès au client est installé et qui doit être utilisé pour obtenir les paramètres de découverte automatique.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Spécifie l’adresse de messagerie à utiliser pour une demande de découverte automatique ultérieure.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Contient le chemin d’accès d’une image utilisée pour personnaliser l’expérience de configuration.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Contient l’URL de la page d’accueil du fournisseur de services Internet (ISP).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur.  <br/> |
|[Erreur (POX)](error-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Réponse (POX)](response-pox.md) <br/> |Contient la réponse du service de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

