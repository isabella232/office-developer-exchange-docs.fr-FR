---
title: Générer une liste des points de terminaison de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 82394d3c-9fc7-4b3c-b48d-1fe983c198f7
description: Découvrez comment générer une liste hiérarchisée des points de terminaison de découverte automatique.
ms.openlocfilehash: ccecacc9c8beef464727efbc9d1fced7a81f9b7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754842"
---
# <a name="generate-a-list-of-autodiscover-endpoints"></a>Générer une liste des points de terminaison de découverte automatique

Découvrez comment générer une liste hiérarchisée des points de terminaison de découverte automatique.
  
La première tâche dans le [processus de découverte automatique](autodiscover-for-exchange.md) consiste à générer une liste des points de terminaison de découverte automatique pour votre application essayer. Ces points de terminaison de découverte automatique peuvent provenir d’une [recherche SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) ou peuvent provenir d’une adresse de messagerie de l’utilisateur. À la fin, vous pouvez vous retrouver avec un grand nombre de points de terminaison. Examinons comment vous pouvez les organiser par priorité. 
  
## <a name="start-with-scp-lookup"></a>Démarrer avec recherche SCP
<a name="bk_StartWithScp"> </a>

Points de terminaison de découverte automatique qui proviennent d’une [recherche SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) doivent avoir la priorité la plus élevée dans votre liste. Les administrateurs peuvent configurer des objets SCP pour router votre client vers le plus proche ou plus efficace découverte automatique du point de terminaison, il est préférable de démarrer avec ces systèmes d’extrémité. Étant donné que le processus de recherche SCP possède son propre schéma de définition des priorités, les résultats d’une recherche SCP sont déjà prioritaire, comme suit : 
  
1. Points de terminaison de découverte automatique des objets SCP étendus au site Active Directory auquel appartient l’ordinateur client.
    
2. Points de terminaison de découverte automatique des objets SCP ne pas étendus à n’importe quel site Active Directory.
    
3. Points de terminaison de découverte automatique des objets SCP étendus à un autre site Active Directory que celui du site auquel appartient l’ordinateur client.
    
Une fois que vous avez les résultats de la recherche SCP, vous pouvez ajouter des points de terminaison dérivés de l’adresse de messagerie de l’utilisateur. Il peuvent être telle qu’une valeur par défaut est définie de points de terminaison et de secours au cas où il n’existe aucun résultat SCP ou les points de terminaison renvoyés par la recherche SCP ne sont pas suffisantes.
  
## <a name="add-endpoints-derived-from-the-users-email-address"></a>Ajouter des points de terminaison dérivés de l’adresse de messagerie de l’utilisateur
<a name="bk_AddDerivedEndpoints"> </a>

Lors de la recherche SCP ne fonctionne pas, ou les points de terminaison renvoyés par la recherche SCP ne renvoient une réponse positive, vous pouvez dériver un ensemble de points de terminaison de découverte automatique par défaut à partir de l’adresse de messagerie de l’utilisateur. Ces points de terminaison doivent être une priorité plus faible que n’importe quel qui proviennent d’une recherche SCP, mais vous devrez peut-être les si la recherche SCP n’a pas réussie.
  
### <a name="to-derive-autodiscover-endpoints"></a>Pour déterminer les points de terminaison de découverte automatique

1. Extraire le nom de domaine à partir de l’adresse de messagerie de l’utilisateur. Par exemple, si l’adresse de messagerie de l’utilisateur est Sadie.Daniels@contoso.com, le nom de domaine serait contoso.com.
    
2. Construire l’URL du point de terminaison sans les extensions de fichiers dans les formats suivants :
    
  - « https:// » + domaine + « autodiscover/autodiscover / »
    
  - "https://autodiscover." + domaine + « autodiscover/autodiscover / »
    
Une fois que vous compilez la liste des URL de point de terminaison dérivés de recherche SCP et adresse de messagerie de l’utilisateur à la fois, vous devrez peut-être modifier les extensions de nom de fichier dans ces URL, selon que vous utilisez le [service web de découverte automatique SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) ou la variole [ Service web de découverte automatique](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).
  
## <a name="add-or-replace-file-name-extensions-in-endpoint-urls"></a>Ajoutez ou remplacez les extensions de nom de fichier dans l’URL du point de terminaison
<a name="bk_FileExtensions"> </a>

Vous pouvez accéder le service de découverte automatique en utilisant le service web de découverte automatique SOAP ou le service web de découverte automatique variole. Chaque service utilise des URL de point de terminaison similaire, avec la seule différence est l’extension de nom de fichier. Le service web de découverte automatique SOAP utilise l’extension de nom de fichier « .svc », et le service web de découverte automatique variole utilise l’extension « .xml ».
  
Par défaut, le point de terminaison de découverte automatique URL renvoyés à partir d’une recherche SCP sont variole URL. Toutefois, si vous utilisez la découverte automatique SOAP, vous pouvez simplement changez l’extension de nom de fichier à partir de « .xml » à « .svc » et essayez une demande SOAP.
  
Pour les URL de point de terminaison de découverte automatique dérivées, l’extension de fichier est omise. Ajoutez l’extension de fichier approprié pour le service web de découverte automatique que vous utilisez avant d’essayer de l’URL.
  
## <a name="example-generating-a-list-of-autodiscover-endpoints"></a>Exemple : Création d’une liste de points de terminaison de découverte automatique
<a name="bk_Example"> </a>

Examinons un exemple. Sadie Daniels (Sadie.Daniels@contoso.com) est l’aide d’une application Exchange Web Services (EWS) pour la première fois. L’application utilise la découverte automatique pour configurer lui-même. Ordinateur de Sadie est joint au domaine contoso.com et se trouve dans le site de Redmond Active Directory. L’application génère la liste des points de terminaison de découverte automatique montre la Figure 1.
  
**La figure 1 : Exemple de liste de points de terminaison de découverte automatique**

![Exemple de liste de points de terminaison de découverte automatique, illustrant des points de terminaison obtenus à partir de la recherche SCP ayant une priorité plus élevée que les points de terminaison dérivés.](media/Ex15_Autodiscover_GenerateList_Example.png)
  
L’application EWS dans cet exemple préfère le service web de découverte automatique SOAP, afin qu’il remplace l’extension de nom de fichier pour les résultats SCP « .svc » avant d’envoyer les demandes SOAP.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_NextSteps"> </a>

Après avoir généré une liste de points de terminaison de découverte automatique, essayez de les en [envoyant des requêtes vers les systèmes d’extrémité](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="see-also"></a>Voir aussi


- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)
    
- [Rechercher des points de terminaison de découverte automatique à l’aide de recherche SCP dans Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    

