---
title: Découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: da0f9402-4e35-42c7-a15e-1e9e4e966e8b
description: En savoir plus sur le service de découverte automatique dans Exchange.
ms.openlocfilehash: f56717eaced5db9028c556c6c2d9aa7794f4988e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754787"
---
# <a name="autodiscover-for-exchange"></a>Découverte automatique pour Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. En savoir plus sur le service de découverte automatique dans Exchange.
  
Le service de découverte automatique d'Exchange offre un moyen facile pour votre application cliente de se configurer elle-même avec une entrée utilisateur minimale. La plupart des utilisateurs connaissent leur adresse de messagerie et leur mot de passe, et avec ces deux informations, vous pouvez récupérer tous les autres détails nécessaires pour être opérationnel. Pour les clients des services web Exchange (EWS), la découverte automatique est généralement utilisée pour rechercher l'URL du point de terminaison EWS. Mais la découverte automatique peut également fournir des informations permettant de configurer les clients qui utilisent d'autres protocoles. Le service de découverte automatique fonctionne pour les applications clientes qui sont à l'intérieur ou à l'extérieur des pare-feu, ainsi que dans des scénarios de forêt de ressources et de forêts multiples.
  
## <a name="overview-of-the-autodiscover-process"></a>Vue d'ensemble du processus de découverte automatique
<a name="bk_Before"> </a>

Le processus de découverte automatique est essentiellement constitué de trois phases. Dans la première phase, vous générez une liste de serveurs de découverte automatique potentiels et au cours de la deuxième phase, vous essayez chaque serveur de votre liste jusqu'à obtenir une réponse positive (espérons-le). Si aucun de vos candidats ne fonctionne, vous passez à la troisième phase, qui représente une tentative de « dernière minute » pour trouver un point de terminaison de découverte automatique.
  
La méthode [ExchangeService.AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) dans l'API managée par EWS implémente les trois phases de ce processus. Ainsi, si vous utilisez l'API managée par EWS, vous n'avez pas à vous soucier de l'implémentation de la découverte automatique. La figure suivante illustre les trois phases du processus de découverte automatique. 
  
**Figure 1. Les trois phases du processus de découverte automatique**

![Illustration du processus de découverte automatique affichant trois phases : définition du pool de candidats, test des points de terminaison et test d'autres alternatives.](media/Ex15_Autodiscover_Overview.png)
  
### <a name="phase-1-defining-the-candidate-pool"></a>Phase 1 : Définition du pool de candidats
<a name="bk_Phase1"> </a>

Avant de pouvoir utiliser la découverte automatique, vous devez localiser le serveur de découverte automatique approprié pour votre utilisateur. Heureusement, la découverte automatique définit un nombre limité d'emplacements de recherche. Si plusieurs candidats sont détectés, la découverte automatique définit également [une méthode pour générer et hiérarchiser la liste](how-to-generate-a-list-of-autodiscover-endpoints.md).
  
**Tableau 1 : Sources de candidats de point de terminaison de découverte automatique**

|**Emplacements de recherche**|**Résultats de la recherche**|
|:-----|:-----|
|Services de domaine Active Directory (AD DS)  <br/> |Pour les clients joints à un domaine, il s'agit du premier emplacement de recherche. Exchange publie des objets de point de connexion de service (SCP) dans AD DS, ce qui permet aux demandes de découverte automatique d'être acheminées vers les serveurs en fonction des sites Active Directory. Les résultats d'une [recherche de SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) doivent être situés en haut de votre liste de candidats.  <br/><br/>**Remarque**: recherche SCP n’est pas disponible pour les clients qui ne sont pas liés à un domaine ou qui n’ont pas accès aux serveurs Active Directory. Dans ce cas, vous devez ignorer la recherche SCP. <br/>|
|Domaine d'adresse de messagerie de l'utilisateur  <br/> | La découverte automatique définit deux formes d'URL de point de terminaison standard dérivées de la partie domaine de l'adresse de messagerie de l'utilisateur :  <br/>`"https://" + domain + "/autodiscover/autodiscover" +  *fileExtension*`  <br/>`"https://autodiscover." + domain + "/autodiscover/autodiscover" +  *fileExtension*`<br/><br/>  La valeur de  *fileExtension*  dépend de la méthode d'accès de découverte automatique que vous utilisez, [SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) ou [POX](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx). Le service SOAP utilise une extension de fichier « .svc » ; POX utilise une extension « .xml ».  <br/> |
   
La figure suivante illustre comment générer une liste de points de terminaison pour la découverte automatique.
  
**Figure 2. Processus de génération d'une liste de points de terminaison pour la découverte automatique**

![Illustration décrivant le processus de génération d'une liste de points de terminaison de découverte automatique. Les flèches indiquent que la liste des points de terminaison est dérivée de la recherche SCP ou de l'adresse de messagerie de l'utilisateur.](media/Ex15_Autodiscover_Overview_Phase1.png)
  
### <a name="phase-2-trying-each-candidate"></a>Phase 2 : Une tentative pour chaque candidat
<a name="bk_Phase2"> </a>

Après avoir généré une liste ordonnée de candidats potentiels, l'étape suivante consiste à essayer chacun de ces candidats figurant sur la liste en [envoyant une demande à l'URL](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et en validant les résultats, comme illustré dans la figure 3. Lorsque vous recevez une réponse positive, l'opération est terminée. 
  
**Figure 3. Une tentative pour chaque candidat de point de terminaison, dans l'ordre**

![Illustration montrant que le serveur recherche chaque point de terminaison selon l'ordre de priorité, jusqu'à ce qu'il reçoive une réponse positive.](media/Ex15_Autodiscover_Overview_Phase2.png)
  
Avant d'envoyer une demande à un candidat, assurez-vous de sa fiabilité. N'oubliez pas que vous envoyez les informations d'identification de l'utilisateur, il est donc important de vérifier que vous les partagez uniquement avec un serveur fiable. Vous devez vérifier au moins les éléments suivants :
  
- Le point de terminaison est un point de terminaison HTTPS. Les applications clientes ne doivent pas être authentifiées ni envoyer des données à un point de terminaison non SSL.
    
- Le certificat SSL envoyé par le serveur est valide et provient d'une autorité approuvée.
    
> [!NOTE]
> [!REMARQUE] Il s'agit uniquement de consignes de sécurité de base. Lorsque vous utilisez une authentification, assurez-vous que le code répond aux exigences de sécurité de votre organisation. 
  
Le type de demande que vous envoyez dépend de la manière dont vous accédez au service de découverte automatique.
  
**Tableau 2. Types de demandes de découverte automatique**

|**Si vous utilisez...**|**Envoyez une demande à l'aide de...**|
|:-----|:-----|
|L'API managée par EWS  <br/> |La méthode [GetUserSettings](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx).  <br/> |
|Le service de découverte automatique SOAP  <br/> |L'opération [GetUserSettings ](http://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx).  <br/> |
|Le service de découverte automatique POX  <br/> |Une demande POST HTTP avec un [corps de demande de service de découverte automatique](http://msdn.microsoft.com/library/75671b1d-f35b-497b-8d8c-706f3f2535fd%28Office.15%29.aspx).  <br/> |
   
### <a name="phase-3-trying-other-alternatives"></a>Phase 3 : Autres solutions
<a name="bk_Phase3"> </a>

Dans certains cas, vous pouvez essayer tous les points de terminaison de votre liste, uniquement pour vous rendre compte qu'ils renvoient tous une erreur. Avant de jeter l'éponge, essayez d'autres méthodes : vous pouvez envoyer une demande GET non authentifiée ou une requête DNS pour un enregistrement SRV. Si ces tentatives ne produisent aucun résultat, vous ne pouvez pas contacter le service de découverte automatique.
  
**Figure 4. Autres solutions**

![Illustration présentant des points de terminaison supplémentaires générés via une demande GET non authentifiée et une requête DNS.](media/Ex15_Autodiscover_Overview_Phase3.png)
  
#### <a name="sending-an-unauthenticated-get-request"></a>Envoi d'une demande GET non authentifiée

La première solution consiste à envoyer une demande GET non authentifiée à un point de terminaison dérivé de l'adresse de messagerie de l'utilisateur. Le format de ce point de terminaison est « http://autodiscover. » + domaine + « /autodiscover/autodiscover.xml ». Notez qu'il ne s'agit pas d'un point de terminaison SSL. Si le serveur renvoie une réponse de redirection 302, vous pouvez ensuite essayer d'[envoyer à nouveau la demande de découverte automatique](handling-autodiscover-error-messages.md#bk_ResendRequest) à l'URL de point de terminaison dans l'en-tête de l'emplacement de la réponse. 
  
#### <a name="querying-dns-for-an-srv-record"></a>Requête DNS pour un enregistrement SRV

Si la demande GET non authentifiée ne fonctionne pas, la dernière chose à essayer est une requête DNS pour les enregistrements SRV du service de découverte automatique. L'enregistrement prend la forme « _autodiscover._tcp. » + domaine. Cette requête peut renvoyer plusieurs enregistrements, mais vous devez utiliser uniquement les enregistrements qui pointent vers un point de terminaison SSL les plus volumineux et avec la priorité la plus élevée.
  
## <a name="options-for-using-autodiscover"></a>Options pour l'utilisation de la découverte automatique
<a name="bk_Options"> </a>

Vous pouvez accéder à la découverte automatique à l'aide du service web POX ou SOAP. La méthode utilisée dépend de vos besoins et de votre environnement. Toutefois, nous vous recommandons d'utiliser le service web SOAP, si possible. L'API managée par EWS est également une option. Elle implémente la partie client des services de découverte automatique SOAP et POX.
  
**Tableau 3 : Options pour accéder au service de découverte automatique**

|**Option**|**Avantages**|**Inconvénients**|
|:-----|:-----|:-----|
|[API managée par EWS](get-started-with-ews-managed-api-client-applications.md) <br/> | Implémente le traitement de découverte automatique pour vous.<br/><br/>Utilise les services de découverte automatique SOAP et POX.<br/><br/>Fonctionne avec Exchange Online, Exchange Online dans le cadre d'Office 365 ou Exchange 2007 SP1, ou une version ultérieure.<br/><br/>Facile à utiliser.  <br/> | Limité au niveau des paramètres utilisateur disponibles dans l'énumération [Microsoft.Exchange.WebServices.Autodiscover.UserSettingName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=EXCHG.80%29.aspx).<br/><br/>Disponible uniquement pour les applications .NET Framework.  <br/> |
|[Découverte automatique SOAP](http://msdn.microsoft.com/library/61c21ea9-7fea-4f56-8ada-bf80e1e6b074%28Office.15%29.aspx) <br/> | Indépendante de la plateforme.<br/><br/>Permet de demander uniquement les paramètres qui vous intéressent.  <br/> | Non disponible dans Exchange 2007.  <br/> |
|[Découverte automatique POX](http://msdn.microsoft.com/library/877152f0-f4b1-4f63-b2ce-924f4bdf2d20%28Office.15%29.aspx) <br/> | Indépendante de la plateforme.<br/><br/>Prise en charge dans Exchange Online et dans Exchange 2007 SP1, ou une version ultérieure.  <br/> | Ne permet pas de demander des paramètres spécifiques.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section

- [Rechercher des points de terminaison de découverte automatique à l’aide de recherche SCP dans Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Générer une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)
    
- [Utiliser la découverte automatique pour rechercher les points de connexion](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Obtenir les paramètres de domaine à partir d’un serveur Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [Actualiser les informations de configuration à l’aide de découverte automatique](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Gestion des messages d'erreur de découverte automatique](handling-autodiscover-error-messages.md)
    
- [Amélioration des performances lors de l'utilisation de la fonctionnalité de découverte automatique pour Exchange](improving-performance-when-using-autodiscover-for-exchange.md)
    
## <a name="see-also"></a>Voir aussi

- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)    
- [Exchange 2013 : Obtenir des paramètres utilisateur avec la découverte automatique](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e)
- [Exemple de vérificateur de découverte automatique](http://code.msdn.microsoft.com/exchange/Autodiscover-Checker-e1ebca42)  
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

