---
title: Actualiser les informations de configuration à l’aide de la découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2f3c6a5-e8ea-4375-b41a-686a6f238d33
description: Découvrez comment et quand actualiser les informations de configuration pour votre connexion Exchange à l’aide de la découverte automatique.
ms.openlocfilehash: b9a4264d150d09b0e143e0bf7365af351bb2ef44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527753"
---
# <a name="refresh-configuration-information-by-using-autodiscover"></a>Actualiser les informations de configuration à l’aide de la découverte automatique

Découvrez comment et quand actualiser les informations de configuration pour votre connexion Exchange à l’aide de la découverte automatique.
  
Lorsque votre application EWS s’exécute pour la première fois, la découverte automatique vous offre un excellent moyen de collecter les informations dont vous avez besoin pour vous connecter à la boîte aux lettres Exchange de votre utilisateur. Toutefois, la découverte automatique n’est pas destinée à être utilisée pour la première fois. L’utilisation régulière de la découverte automatique permet de maintenir votre application connectée en lui permettant de répondre aux modifications apportées au déploiement d’Exchange.
  
## <a name="cache-autodiscover-endpoint-and-ews-settings"></a>Mettre en cache le point de terminaison de découverte automatique et les paramètres EWS
<a name="bk_CacheSettings"> </a>

Bien que nous vous recommandons d’utiliser la découverte automatique régulièrement, l’utilisation régulière de celle-ci nécessite une attention particulière. Idéalement, vous pouvez équilibrer le temps de réponse aux modifications apportées à l’environnement contre la génération d’un trafic réseau superflu. Lorsque votre application obtient une réponse de découverte automatique pour la première fois, vous devez enregistrer les informations suivantes afin de ne pas avoir à répéter le processus de découverte automatique à chaque fois que vous envoyez une demande EWS.
  
**Tableau 1. Informations à mettre en cache pour les demandes de découverte automatique**

|**Définition à mettre en cache**|**Valide pour...**|**Détails**|
|:-----|:-----|:-----|
|Point de terminaison de découverte automatique  <br/> |Tant qu’elle fonctionne  <br/> |Lorsque vous enregistrez le point de terminaison de découverte automatique qui a renvoyé une réponse réussie, il n’est pas nécessaire de répéter le processus de [génération d’une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md) et de les essayer jusqu’à ce que vous obteniez une réponse réussie.<br/><br/> **Remarque**: l’API managée EWS ne prend pas en charge la mise en cache du point de terminaison de découverte automatique.           |
|URL EWS et tous les autres paramètres récupérés à partir de la réponse de découverte automatique  <br/> |Une semaine  <br/> |En enregistrant l’URL EWS et d’autres paramètres associés, vous n’avez pas besoin d' [Envoyer une nouvelle demande de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) pour chaque demande EWS ou si votre application redémarre. Toutefois, même si une URL EWS fonctionne pour votre utilisateur, un serveur peut être disponible plus ou moins.<br/><br/> Par exemple, la boîte aux lettres de l’utilisateur a peut-être été déplacée vers un nouveau serveur de boîtes aux lettres, ce qui se traduit par un nouveau point de terminaison EWS. Nous vous recommandons d’actualiser vos paramètres utilisateur en envoyant une nouvelle demande de découverte automatique après une semaine passée depuis votre dernière demande de découverte automatique. Cette durée peut être ajustée pour répondre aux exigences de votre application.  <br/> |
   
## <a name="refresh-cached-configuration-information"></a>Actualiser les informations de configuration mises en cache
<a name="bk_RefreshConfig"> </a>

Maintenant que vous disposez des informations mises en cache, examinons comment vous pouvez conserver ce cache à jour. Nous vous recommandons d’actualiser vos informations mises en cache lorsque :
  
- La période de validité de l’information expire.
    
- Une [erreur liée à la connexion](#bk_ConnectionErrors) se produit et les informations mises en cache ont été actualisées pour la dernière fois il y a une heure.
    
Pour actualiser vos informations mises en cache, envoyez une demande de découverte automatique à un point de terminaison de découverte automatique mis en cache, puis procédez comme suit :
  
- Si la demande aboutit, comparez le point de terminaison EWS dans la réponse au point de terminaison EWS mis en cache et procédez comme suit :
    
  - S’ils sont différents, utilisez le nouveau point de terminaison EWS. Si vous effectuez une actualisation afin de récupérer suite à une erreur, renouvelez la demande ayant échoué avec le nouveau point de terminaison.
    
  - S’ils sont identiques, continuez à utiliser le point de terminaison EWS d’origine. Si vous effectuez une actualisation afin de récupérer suite à une erreur, gérez l’erreur comme il convient.
    
- En cas d’échec de la demande, démarrez le [processus de découverte automatique](autodiscover-for-exchange.md) depuis le début. Une fois que vous obtenez une réponse réussie, remplacez le point de terminaison de découverte automatique mis en cache par le point de terminaison de découverte automatique qui a réussi et continuer à utiliser le nouveau point de terminaison EWS. Si vous ne recevez pas de réponse, continuez à utiliser le point de terminaison de découverte automatique d’origine et le point de terminaison EWS. Si vous effectuez une actualisation afin de récupérer suite à une erreur, gérez l’erreur comme il convient. 
    
La figure suivante fournit une représentation visuelle de ce processus.
  
**Figure 1. Processus d’actualisation des informations de configuration à l’aide de la découverte automatique**

![Diagramme schématique indiquant comment la découverte automatique actualise les informations de configuration.](media/Ex15_Autodiscover_Refresh_Flowchart.png)
  
### <a name="connection-related-errors"></a>Erreurs liées à la connexion
<a name="bk_ConnectionErrors"> </a>

L’actualisation des informations de configuration mises en cache peut vous aider à résoudre certaines erreurs, mais pas toutes. 
  
**Tableau 2. Erreurs à résoudre en actualisant votre cache**

|**Error**|**Implémentation de l’API managée EWS**|**Remarques**|
|:-----|:-----|:-----|
|Erreurs de défaillance du réseau ou du DNS<br/><br/> Exemple : le nom d’hôte est introuvable.  <br/> |[ServiceRemoteException](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Toute erreur indiquant que le serveur est introuvable ou inaccessible peut être résolue en tentant la découverte automatique. <br/><br/> Le point de terminaison EWS mis en cache n’est peut-être plus valide et la découverte automatique peut vous faire pointer vers le nouveau serveur.  <br/> |
|Erreurs d’état HTTP<br/><br/> Exemple : service 503 indisponible  <br/> |[ServiceRemoteException](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.serviceremoteexception?view=exchange-ews-api) <br/> |Des erreurs d’état HTTP peuvent se produire pour de nombreuses raisons.<br/><br/> Toutefois, il est recommandé d’essayer la découverte automatique pour voir si un nouveau point de terminaison EWS est disponible pour l’utilisateur.  <br/> |
|Codes d’erreur EWS <br/><br/> Exemple : ErrorConnectionFailed <br/> |[ResponseCodeType](../web-service-reference/responsecode.md) <br/> | La plupart des codes d’erreur EWS ne justifient pas l’actualisation de vos informations de configuration.<br/><br/> Toutefois, les éléments suivants indiquent spécifiquement que les informations de configuration doivent être mises à jour :<br/>- **ErrorConnectionFailed** <br/>- **ErrorMailboxMoveInProgress** <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)  
- [Générer une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

