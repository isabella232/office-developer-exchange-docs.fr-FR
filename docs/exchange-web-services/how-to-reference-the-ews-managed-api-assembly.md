---
title: Référencer l'assembly d'API managée EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 130990db-6297-42dc-9f5d-f68a2400872a
description: Découvrez comment référencer l'assembly d'API managée EWS.
localization_priority: Priority
ms.openlocfilehash: d49091781da279d87a1eab35608f19ece43a0333
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527760"
---
# <a name="reference-the-ews-managed-api-assembly"></a>Référencer l'assembly d'API managée EWS

Découvrez comment référencer l'assembly d'API managée EWS.
  
L'API managée EWS fournit une interface simple et complète pour développer et étendre les applications qui utilisent les services web Exchange (EWS). Que vous utilisiez Visual Studio ou un autre éditeur de code pour développer votre application API managée EWS, vous aurez besoin de faire référence à l'assembly API managée EWS. Si vous n'avez pas encore installé l'API managée EWS, [téléchargez-la](https://aka.ms/ews-managed-api-readme).
  
> [!NOTE]
> L’API managée EWS est désormais disponible comme projet open source sur [GitHub](https://github.com/officedev/ews-managed-api). Vous pouvez utiliser la bibliothèque open source pour : 
> - Participer aux résolutions de bogues et aux améliorations de l’API. 
> - obtenir des correctifs et des améliorations avant qu’ils soient disponibles dans une version officielle ; 
> - Accéder à l’implémentation la plus complète et la plus à jour de l’API afin de l’utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes.
> 
>  Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) sont les bienvenues via GitHub. 
  
## <a name="referencing-the-assembly"></a>Référencer l’assembly

La façon la plus courante d'ajouter une référence est d'utiliser Visual Studio. Nous savons que certains développeurs préfèrent utiliser d'autres éditeurs, donc nous allons vous donner des instructions pour utiliser le compilateur de ligne de commande, ainsi que des instructions pour l'utilisation de Visual Studio. Vous remarquerez que les exemples de code qui suivent présentent les mêmes instructions **using**. La différence entre les deux méthodes est que le compilateur de ligne de commande a besoin de l'emplacement du fichier d'assembly. La référence Visual Studio s'occupe de cela pour vous en arrière-plan. 
  
### <a name="to-add-a-reference-by-using-visual-studio"></a>Pour ajouter une référence à l'aide de Visual Studio

1. Placez le fichier Microsoft.Exchange.WebServices.dll et le fichier Microsoft.Exchange.WebServices.xml dans un dossier de votre choix. Par défaut, les fichiers sont installés dans  `C:\Program Files\Microsoft\Exchange\Web Services\2.0\`, mais vous pouvez les stocker où vous voulez sur votre ordinateur.
    
2. Dans le volet Explorateur de solutions dans Visual Studio, sélectionnez **Références**, puis choisissez **Ajouter une référence**. La fenêtre Ajouter une référence s'ouvre.
    
3. Dans la fenêtre Ajouter une référence, accédez à l'onglet **Parcourir**, puis à l'emplacement du fichier Microsoft.Exchange.WebServices.dll, sélectionnez ce fichier, puis sélectionnez **OK**. 
    
4. Pour utiliser l'API managée EWS dans votre application, ajoutez une instruction **using** pour l'espace de noms **Microsoft.Exchange.WebServices.Data**. 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

### <a name="to-add-a-reference-and-build-your-application-with-the-command-line-compiler"></a>Pour ajouter une référence et créer votre application avec le compilateur de ligne de commande

1. Placez le fichier Microsoft.Exchange.WebServices.dll dans un dossier de votre choix. Ce dossier sera le dossier de sortie pour le compilateur.
    
2. Dans votre éditeur de code source, ajoutez une instruction **using** au code source pour l'espace de noms **Microsoft.Exchange.WebServices.Data**. 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

3. Exécutez le compilateur de ligne de commande pour créer l'application. La commande suivante utilise le compilateur C# .NET Framework pour créer l'application Windows définie dans le fichier de code source « program.cs ». Il suppose que le compilateur se trouve dans le répertoire d'installation par défaut et que le fichier Microsoft.Exchange.WebServices.dll est dans un sous-répertoire du répertoire en cours appelé « build ».
    
   ```cs
    c:\Windows\Microsoft.NET\Framework\3.5\csc /target: winexe /out: build\testApplication /reference: build\Microsoft.Exchange.WebServices.dll program.cs
   ```

## <a name="see-also"></a>Voir aussi

- [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md)    
- [Configuration de votre environnement de développement d’application Exchange](setting-up-your-exchange-application-development-environment.md)   
- [Communiquer avec EWS à l'aide de l'API managée EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    

