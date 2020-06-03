---
title: Configuration de votre environnement de développement d’application Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 91b86e93-bdde-41c3-9680-45cf61420592
description: Découvrez comment configurer votre environnement de développement pour créer une application EWS qui communique avec Exchange.
localization_priority: Priority
ms.openlocfilehash: 01a106817f29bd696991b8a0c5d7d9b7dd420b94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463761"
---
# <a name="setting-up-your-exchange-application-development-environment"></a>Configuration de votre environnement de développement d’application Exchange

Découvrez comment configurer votre environnement de développement pour créer une application EWS qui communique avec Exchange.
  
Avant de commencer à écrire votre application services Web Exchange (EWS), vous devez vous assurer que votre environnement de développement répond à quelques exigences minimum. Vous pouvez utiliser l’API managée EWS, l’API d’accès au client standard pour les applications .NET Framework, pour développer votre application ou vous pouvez utiliser EWS en tant que tel, avec notre sans proxy autogénéré. En général, nous vous recommandons d’utiliser l’API managée EWS ; Toutefois, vous pouvez [Explorer la différence entre ces deux options](ews-client-design-overview-for-exchange.md) plus en détail pour savoir laquelle est la plus adaptée pour vous. 
  
> [!NOTE]
> L’API managée EWS est désormais disponible comme projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source pour : 
> - Participer aux résolutions de bogues et aux améliorations de l’API. 
> - obtenir des correctifs et des améliorations avant qu’ils soient disponibles dans une version officielle ; 
> - Accéder à l’implémentation la plus complète et la plus à jour de l’API afin de l’utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes.
> 
>  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) sont les bienvenues via GitHub. 
  
## <a name="development-environment-for-the-ews-managed-api"></a>Environnement de développement pour l’API managée EWS
<a name="bk_EWSMA"> </a>

Pour créer une application d’API managée EWS, vous devez accéder aux éléments suivants :
  
- L'[API managée EWS](https://aka.ms/ews-managed-api-readme). 
    
    Vous pouvez stocker les fichiers de l’API managée EWS n’importe où sur votre ordinateur ; par défaut, ils sont installés dans le dossier Program Files\Microsoft\Exchange\Web services \\<numéro de version \> .
    
- Une boîte aux lettres sur un serveur Exchange qui exécute Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version d’Exchange à partir d’Exchange Server 2007. 
    
    Vous pouvez obtenir un plan Exchange Online pour les entreprises, y compris une version d’évaluation gratuite, à partir du [site Office 365](https://office.microsoft.com/business/compare-office-365-for-business-plans-FX102918419.aspx#fbid=1tsGNIE7e3a). Pour vous connecter à la boîte aux lettres, vous devez posséder le nom d’utilisateur et les informations d’identification du compte associé à la boîte aux lettres.

    
- Une version de Visual Studio à partir de Visual Studio 2005. Si vous ne disposez pas de Visual Studio, vous pouvez télécharger une [version gratuite](https://visualstudio.microsoft.com/).
    
- Une version de .NET Framework à partir de .NET Framework 3,5. Vous pouvez télécharger .NET Framework 3,5 à partir du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/?LinkId=191777).
    
Par ailleurs, il est utile si vous êtes familiarisé avec C#. Bien que Visual Studio prenne en charge d’autres langages en plus de C#, la plupart des exemples de code disponibles pour l’API managée EWS sont écrits en C#.
  
## <a name="development-environment-for-ews"></a>Environnement de développement pour EWS
<a name="bk_EWS"> </a>

Vous pouvez utiliser EWS pour développer votre application de deux manières différentes. La manière la plus simple d’utiliser EWS est de créer des fichiers texte contenant vos requêtes XML et de les transmettre à Exchange. Pour ce faire, voici ce dont vous avez besoin : 
  
- Un simple éditeur de texte, tel que le bloc-notes, pour modifier votre demande XML. Tout éditeur de texte fera, même si vous en aurez besoin pour la validation de la syntaxe XML, comme XMetal.
    
- Outil ou application pouvant envoyer et recevoir des demandes et des réponses XML SOAP afin de communiquer avec Exchange.
    
Lorsque vous utilisez du code XML brut, il est également utile de posséder une compréhension de base de la mise en forme XML.
  
La deuxième façon d’utiliser EWS est de créer un proxy généré automatiquement qui vous permet d’utiliser les opérations à l’aide d’un langage .NET comme C#. Voici ce dont vous avez besoin pour utiliser un proxy généré automatiquement :
  
- Une version de Visual Studio à partir de Visual Studio 2005, pour créer une référence de proxy. Vous pouvez télécharger une [version gratuite](https://visualstudio.microsoft.com/).
    
- Une version de .NET Framework à partir de .NET Framework 2,0. Vous pouvez télécharger .NET Framework 3,5 à partir du [Centre de téléchargement Microsoft](https://go.microsoft.com/fwlink/?LinkId=191777).
    
Si vous utilisez un proxy généré automatiquement, vous souhaiterez être familiarisé avec la programmation C#.
  
> [!NOTE]
> Si vous êtes développeur .NET Framework, nous vous encourageons à utiliser l’API managée EWS plutôt que les proxies autogénérés pour développer sur EWS. Le modèle objet de l’API managée EWS est plus facile à utiliser que les modèles objet de proxy autogénérés. Par ailleurs, l’API managée EWS implémente la [découverte automatique](autodiscover-for-exchange.md) et inclut une logique côté client. 
  
## <a name="see-also"></a>Voir aussi

- [Configuration de votre environnement de développement d’application Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)  
- [Contrôler l’accès à EWS dans Exchange](how-to-control-access-to-ews-in-exchange.md)  
- [Modèles d’objet générés par EWS pour Exchange](https://msdn.microsoft.com/library/jj190899)
    