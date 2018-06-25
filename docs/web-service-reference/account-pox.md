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
description: L’élément compte Spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: 88911aad41816f7cefbffef151e066fe5d4da192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756321"
---
# <a name="account-pox"></a>Compte (POX)

L’élément **compte** spécifie les paramètres de compte pour l’utilisateur ou contient des réponses d’erreur. 
  
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
|[Protocole (POX)](protocol-pox.md) <br/> |Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.  <br/> |
|[Erreur (POX)](error-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Réponse (POX)](response-pox.md) <br/> |Contient la réponse du service de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

