---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: L’élément compte Spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353342"
---
# <a name="account-pox"></a>Account (POX)

L’élément **compte** spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
- [Response (POX)](response-pox.md)
- [Account (POX)](account-pox.md)
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Représente le type de compte.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Fournit des informations qui sont utilisées pour déterminer si une autre requête de découverte automatique est requise pour retourner les informations de configuration utilisateur.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Contient une valeur qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre d’Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Contient l’URL de l’ordinateur qui exécute le serveur Exchange qui a le rôle de serveur Client Access installé qui doit être utilisé pour obtenir les paramètres de découverte automatique.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Spécifie l’adresse de messagerie qui doit être utilisé pour une requête de découverte automatique suivante.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Contient le chemin d’accès d’une image qui est utilisée pour personnaliser l’expérience de configuration.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Contient l’URL de la page d’accueil du fournisseur de services Internet (fournisseur de services Internet).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.  <br/> |
|[Erreur (POX)](error-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Contient la réponse du service de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

