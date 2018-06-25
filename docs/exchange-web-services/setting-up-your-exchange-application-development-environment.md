---
title: La configuration de votre environnement de développement d’application Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: Découvrez comment configurer votre environnement de développement pour créer une application EWS qui communique avec Exchange.
ms.openlocfilehash: 0c7d4c6d37b28b6797bdb638930b8582f31ffc5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755067"
---
# <a name="setting-up-your-exchange-application-development-environment"></a>La configuration de votre environnement de développement d’application Exchange

Découvrez comment configurer votre environnement de développement pour créer une application EWS qui communique avec Exchange.
  
Avant de commencer à écrire votre application Exchange Web Services (EWS), vous devez vous assurer que votre environnement de développement présente quelques configuration minimale requise. Vous pouvez utiliser l’API managée EWS, l’API d’accès client standard pour les applications .NET Framework, pour développer votre application, ou vous pouvez utiliser EWS sur son propre, avec notre sans un proxy généré automatiquement. En général, nous vous recommandons d’utiliser l’API managée EWS ; Toutefois, vous pouvez [Explorer la différence entre ces deux options](ews-client-design-overview-for-exchange.md) plus en détail pour rechercher les est fait pour vous. 
  
> [!NOTE]
>  [!REMARQUE]  L'API managée EWS est maintenant disponible en tant que projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source pour : >  participer aux résolutions de bogues et aux améliorations apportées à l'API ; >  obtenir des correctifs et des améliorations avant qu'ils soient disponibles dans une version officielle ; >  accéder à l'implémentation la plus complète et la plus à jour de l'API, afin de l'utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes. >  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub sont les bienvenues. 
  
## <a name="development-environment-for-the-ews-managed-api"></a>Environnement de développement pour l’API managée EWS
<a name="bk_EWSMA"> </a>

Pour créer une application d’API managées, vous devez avoir accès à ce qui suit :
  
- L'[API managée EWS](http://aka.ms/ews-managed-api-readme). 
    
    Vous pouvez stocker les fichiers de l’API managée EWS n’importe où sur votre ordinateur ; par défaut, ils sont installés dans les Services Files\Microsoft\Exchange\Web\\< numéro de version\> dossier.
    
- Une boîte aux lettres sur un serveur Exchange qui exécute Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange commençant par Exchange Server 2007. 
    
    Vous pouvez obtenir un plan Exchange Online pour les entreprises, y compris une version d’évaluation gratuite, à partir du [site Office 365](http://office.microsoft.com/en-us/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a). Pour pouvoir se connecter à la boîte aux lettres, vous devez disposer du nom d’utilisateur et les informations d’identification du compte associé à la boîte aux lettres.
    
- Une version de Visual Studio commençant par Visual Studio 2005. Si vous ne disposez pas de Visual Studio, vous pouvez télécharger une version gratuite de [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).
    
- Une version du .NET Framework commençant par le .NET Framework 3.5. Vous pouvez télécharger le .NET Framework 3.5 à partir du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/?LinkId=191777).
    
En outre, il est utile si vous être familiarisé avec c#. Bien que Visual Studio prend en charge les autres langues en plus de Visual C#, la plupart des exemples de code disponibles pour l’API managée EWS est écrit en c#.
  
## <a name="development-environment-for-ews"></a>Environnement de développement pour EWS
<a name="bk_EWS"> </a>

Vous pouvez utiliser EWS pour développer votre application de deux manières différentes. La façon la plus simple d’utiliser EWS consiste à créer des fichiers texte qui contiennent des demandes de votre XML et de les transmettre à Exchange. Pour ce faire, voici ce que vous devez : 
  
- Un simple éditeur de texte tel que le bloc-notes, pour modifier votre requête XML. N’importe quel éditeur de texte fera, bien que vous pouvez souhaiter une qui vous aideront à votre validation de la syntaxe XML comme XMetal.
    
- Un outil ou une application qui peut envoyer et recevoir des demandes SOAP XML et des réponses, afin de pouvoir communiquer avec Exchange.
    
Lorsque vous travaillez avec le code XML brut, il est également utile d’avoir une connaissance élémentaire de mise en forme XML.
  
Utiliser EWS, la deuxième consiste à créer un proxy généré automatiquement qui vous permet de travailler avec les opérations à l’aide d’un langage .NET tel que c#. Voici ce que vous devez utiliser un proxy généré automatiquement :
  
- Une version de Visual Studio commençant par Visual Studio 2005, pour créer une référence au serveur proxy. Vous pouvez télécharger une version gratuite de [Visual Studio 2010 Express](http://www.microsoft.com/visualstudio/eng/products/visual-studio-2010-express).
    
- Une version du .NET Framework commençant par le .NET Framework 2.0. Vous pouvez télécharger le .NET Framework 3.5 à partir du [Centre de téléchargement Microsoft](http://go.microsoft.com/fwlink/?LinkId=191777).
    
Si vous utilisez un proxy généré automatiquement, vous souhaiterez être familiarisé avec la programmation c#.
  
> [!NOTE]
> Si vous êtes un développeur .NET Framework, nous vous conseillons d’utiliser l’API managées plutôt que des serveurs proxy généré automatiquement pour développer avec EWS. Le modèle objet d’API managées est plus facile à utiliser que les modèles objet de proxy généré automatiquement. En outre, l’API managée EWS implémente la [découverte automatique](autodiscover-for-exchange.md) et inclut une logique côté client. 
  
## <a name="see-also"></a>Voir aussi


- [La configuration de votre environnement de développement d'applications Exchange](setting-up-your-exchange-application-development-environment.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [Contrôler l’accès à EWS dans Exchange](how-to-control-access-to-ews-in-exchange.md)
    
- [EWS généré des modèles objet pour Exchange](https://msdn.microsoft.com/en-us/library/jj190899)
    

