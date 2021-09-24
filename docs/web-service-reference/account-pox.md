---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: L’élément Account spécifie les paramètres de compte de l’utilisateur ou contient des réponses d’erreur.
ms.openlocfilehash: 89799ab62a2aa4945b0e8f3209ab1fbc7d2fa2e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534052"
---
# <a name="account-pox"></a>Account (POX)

**L’élément Account** spécifie les paramètres de compte de l’utilisateur ou contient des réponses d’erreur. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AccountType (POX)](accounttype-pox.md) <br/> |Représente le type de compte.  <br/> |
|[Action (POX)](action-pox.md) <br/> |Fournit des informations qui sont utilisées pour déterminer si une autre demande de découverte automatique est nécessaire pour renvoyer les informations de configuration utilisateur.  <br/> |
|[MicrosoftOnline (POX)](microsoftonline-pox.md) <br/> |Contient une valeur qui indique si la boîte aux lettres de l’utilisateur est hébergée dans Exchange Online ou Exchange Online dans le cadre Office 365.  <br/> |
|[RedirectUrl (POX)](redirecturl-pox.md) <br/> |Contient l’URL de l’ordinateur qui exécute Exchange Server sur le rôle serveur d’accès au client qui doit être utilisé pour obtenir les paramètres de découverte automatique.  <br/> |
|[RedirectAddr (POX)](redirectaddr-pox.md) <br/> |Spécifie l’adresse de messagerie à utiliser pour une demande de découverte automatique ultérieure.  <br/> |
|[Image (POX)](image-pox.md) <br/> |Contient le chemin d’accès d’une image utilisée pour brander l’expérience de configuration.  <br/> |
|[ServiceHome (POX)](servicehome-pox.md) <br/> |Contient l’URL de la page d’accueil du fournisseur de services Internet (ISP).  <br/> |
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client au serveur d’accès au client.  <br/> |
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir des informations de dossier public pour l’utilisateur.  <br/> |
|[Erreur (POX)](error-pox.md) <br/> |Contient une réponse d’erreur de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Response (POX)](response-pox.md) <br/> |Contient la réponse du service de découverte automatique.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

