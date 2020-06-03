---
title: Générer une liste de points de terminaison de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 82394d3c-9fc7-4b3c-b48d-1fe983c198f7
description: Découvrez comment générer une liste de points de terminaison de découverte automatique classés par ordre de priorité.
localization_priority: Priority
ms.openlocfilehash: db888c8d562f57bd46edc251f4917e9e03d85d95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528098"
---
# <a name="generate-a-list-of-autodiscover-endpoints"></a>Générer une liste de points de terminaison de découverte automatique

Découvrez comment générer une liste de points de terminaison de découverte automatique classés par ordre de priorité.
  
La première tâche du [processus de découverte automatique](autodiscover-for-exchange.md) consiste à générer une liste de points de terminaison de découverte automatique à essayer par votre application. Ces points de terminaison de découverte automatique peuvent provenir d’une [recherche SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) ou être dérivés de l’adresse de messagerie de l’utilisateur. À la fin, vous pouvez obtenir un grand nombre de points de terminaison. Examinons comment vous pouvez les organiser par priorité. 
  
## <a name="start-with-scp-lookup"></a>Commencer avec la recherche SCP
<a name="bk_StartWithScp"> </a>

Les points de terminaison de découverte automatique provenant d’une [recherche SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) doivent avoir la priorité la plus haute dans votre liste. Les administrateurs peuvent configurer les objets SCP pour acheminer votre client vers le point de terminaison de découverte automatique le plus proche ou le plus efficace, il est donc judicieux de commencer avec ces points de terminaison. Étant donné que le processus de recherche SCP a son propre schéma de définition des priorités, les résultats d’une recherche SCP sont déjà prioritaires, comme suit : 
  
1. Points de terminaison de découverte automatique des objets SCP inclus dans l’étendue du site Active Directory auquel appartient l’ordinateur client.
    
2. Les points de terminaison de découverte automatique des objets SCP ne sont inclus dans aucun site Active Directory.
    
3. Les points de terminaison de découverte automatique des objets SCP dont l’étendue est limitée à un site Active Directory différent du site auquel appartient l’ordinateur client.
    
Une fois que vous avez obtenu les résultats du processus de recherche SCP, vous pouvez ajouter des points de terminaison qui dérivent de l’adresse de messagerie de l’utilisateur. Ces éléments peuvent servir de jeu par défaut de points de terminaison et de secours s’il n’y a aucun résultat SCP ou si les points de terminaison renvoyés par la recherche SCP ne sont pas suffisants.
  
## <a name="add-endpoints-derived-from-the-users-email-address"></a>Ajouter des points de terminaison dérivés de l’adresse de messagerie de l’utilisateur
<a name="bk_AddDerivedEndpoints"> </a>

Lorsque la recherche SCP ne fonctionne pas ou que les points de terminaison renvoyés par la recherche SCP ne renvoient pas de réponse correcte, vous pouvez dériver un ensemble de points de terminaison de découverte automatique par défaut à partir de l’adresse de messagerie de l’utilisateur. Ces points de terminaison doivent être moins prioritaires que ceux provenant d’une recherche SCP, mais vous en aurez peut-être besoin si la recherche SCP n’a pas réussi.
  
### <a name="to-derive-autodiscover-endpoints"></a>Pour dériver des points de terminaison de découverte automatique

1. Extrayez le nom de domaine de l’adresse de messagerie de l’utilisateur. Par exemple, si l’adresse de messagerie de l’utilisateur est Sadie.Daniels@contoso.com, le nom de domaine est contoso.com.
    
2. Créez des URL de point de terminaison sans extensions de fichiers aux formats suivants :
    
  - « https:// » + domaine + « /autodiscover/autodiscover »
    
  - "https://autodiscover." + domaine + « /autodiscover/autodiscover »
    
Une fois que vous avez compilé la liste des URL de point de terminaison qui dérivent de la recherche SCP et de l’adresse de messagerie de l’utilisateur, vous devrez peut-être réviser les extensions de nom de fichier dans ces URL, selon que vous utilisez le [service Web de découverte automatique SOAP](https://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) ou le [service Web de découverte automatique pox](https://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx).
  
## <a name="add-or-replace-file-name-extensions-in-endpoint-urls"></a>Ajouter ou remplacer des extensions de nom de fichier dans les URL de point de terminaison
<a name="bk_FileExtensions"> </a>

Vous pouvez accéder au service de découverte automatique en utilisant le service Web de découverte automatique SOAP ou le service Web de découverte automatique POX. Chaque service utilise des URL de point de terminaison similaires, la seule différence étant l’extension de nom de fichier. Le service Web de découverte automatique SOAP utilise l’extension de nom de fichier « . svc » et le service Web de découverte automatique POX utilise l’extension de nom de fichier « . Xml ».
  
Par défaut, les URL du point de terminaison de découverte automatique renvoyées par une recherche SCP sont des URL de POX. Toutefois, si vous utilisez la découverte automatique SOAP, il vous suffit de remplacer l’extension de nom de fichier « . xml » par « . svc » et d’essayer une demande SOAP.
  
Pour les URL de point de terminaison de découverte automatique dérivées, l’extension de fichier est omise. Ajoutez l’extension de fichier appropriée pour le service Web de découverte automatique que vous utilisez avant de tester l’URL.
  
## <a name="example-generating-a-list-of-autodiscover-endpoints"></a>Exemple : génération d’une liste de points de terminaison de découverte automatique
<a name="bk_Example"> </a>

Examinons un exemple. Sadie Daniels (Sadie.Daniels@contoso.com) utilise une application services Web Exchange (EWS) pour la première fois. L’application utilise la découverte automatique pour se configurer elle-même. L’ordinateur de Sadie est joint au domaine contoso.com et se trouve dans le site Active Directory de Redmond. L’application génère la liste des points de terminaison de découverte automatique illustrée dans la figure 1.
  
**Figure 1 : exemple de liste de points de terminaison de découverte automatique**

![Exemple de liste de points de terminaison de découverte automatique, illustrant des points de terminaison obtenus à partir de la recherche SCP ayant une priorité plus élevée que les points de terminaison dérivés.](media/Ex15_Autodiscover_GenerateList_Example.png)
  
Dans cet exemple, l’application EWS préfère le service Web de découverte automatique SOAP, de sorte qu’elle modifie l’extension de nom de fichier pour les résultats SCP en « . svc » avant d’envoyer des demandes SOAP à ces derniers.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_NextSteps"> </a>

Une fois que vous avez généré une liste de points de terminaison de découverte automatique, essayez-les en [envoyant des demandes à ces points de terminaison](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="see-also"></a>Voir aussi


- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)
    
- [Trouver des points de terminaison de découverte automatique à l’aide de la recherche SCP dans Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    

