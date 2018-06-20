---
title: Accéder aux dossiers publics avec EWS dans Exchange
manager: sethgros
ms.date: 7/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d9372057-1deb-45de-8f98-b9149604429a
description: Découvrez comment utiliser EWS et l’API managée EWS pour accéder aux dossiers publics et router les demandes de dossiers publics dans Exchange.
ms.openlocfilehash: cfa089ba617dc760ed12883590e141debb5ecd9b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755068"
---
# <a name="public-folder-access-with-ews-in-exchange"></a>Accéder aux dossiers publics avec EWS dans Exchange

Découvrez comment utiliser EWS et l’API managée EWS pour accéder aux dossiers publics et router les demandes de dossiers publics dans Exchange.
  
Les dossiers publics fournissent un référentiel partagé d’éléments que les utilisateurs de votre organisation peuvent accéder. Office 365, Exchange Online et les versions locales d’Exchange commençant par Exchange 2013 introduisent une nouvelle architecture pour les dossiers publics. Dossiers publics dans Exchange utilisent une conception de boîtes aux lettres spécialisés (au lieu d’une base de données de dossier public) pour stocker la hiérarchie de dossiers publics et le contenu des dossiers publics. Autorisations de dossiers publics sont gérées par le biais de rôle en fonction de contrôle d’accès (RBAC).
  
Technologies d’accès client, tels que Exchange Web Services (EWS) et l’API managée EWS, fournissent l’accès par programme à la hiérarchie de dossiers publics et les éléments de contenu dans une base de données de dossiers publics. Cet article fournit des informations sur la façon dont vous pouvez utiliser EWS et l’API managée EWS pour accéder aux dossiers publics et les dossiers publics et les données de dossiers publics. 
  
## <a name="ews-operations-and-ews-managed-api-methods-for-public-folder-access"></a>Opérations EWS et méthodes d’API managées pour accéder aux dossiers publics
<a name="bk_functionality"> </a>

La plupart des opérations EWS principaux prend en charge l’accès aux dossiers publics. Vous pouvez utiliser les opérations de dossier et élément et les méthodes API managées répertoriés dans le tableau suivant pour travailler avec les dossiers publics.
  
Pour plus d’informations sur les méthodes de l’API managée EWS, voir [espaces de noms API managées](http://msdn.microsoft.com/en-us/library/jj220535%28v=exchg.80%29.aspx).
  
|**Opération EWS**|**Méthode d'API managée EWS**|
|:-----|:-----|
|[Opération CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |**Folder.Save()** <br/> |
|[Opération UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |**Folder.Update()** <br/> |
|[Opération DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |**Folder.Delete()** <br/> |
|[Opération MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <sup>1</sup> <br/> |**Folder.Move()** <br/> |
|[Opération CopyFolder](http://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <sup>2</sup> <br/> |**Folder.Copy()** <br/> |
|[Opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |**Folder.Bind()** <br/> |
|[Opération EmptyFolder](http://msdn.microsoft.com/library/98161486-e2f2-480f-8d5d-708ba81b208a%28Office.15%29.aspx) <sup>3</sup> <br/> |**Folder.Empty()** <br/> |
|[Opération FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |**ExchangeService.FindFolders()** <br/> **Folder.FindFolders()** <br/> |
|[CreateItem Operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> |**Item.Save()** <br/> |
|[Opération MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |**Item.Move()** <br/> |
|[Opération CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |**Item.Copy()** <br/> |
|[UpdateItem Operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |**Item.Update()** <br/> |
|[Opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |**Item.Delete()** <br/> |
|[Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <sup>4</sup> <br/> |**ExchangeService.FindItems()** <br/> **Folder.FindItems()** <br/> |
|[GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |**Item.Bind()** <br/> |
|[Opération ConvertId](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx) <sup>5</sup> <br/> |**ExchangeService.ConvertId()** <br/> **ExchangeService.ConvertIds()** <br/> |
   
<sup>1</sup> la déplacer des dossiers entre un dossier privé et un dossier public n’est pas disponible dans les versions d’Exchange commençant par Exchange 2013. 
  
<sup>2</sup> cette opération n’est applicable aux dossiers publics dans Exchange Server 2007 et Exchange Server 2010. 
  
<sup>3</sup> cette opération n’est applicable aux dossiers publics dans Exchange 2010. 
  
<sup>4</sup> recherche indexés dans un dossier public via l’option de chaîne de requête de recherche en texte intégral est pris en charge dans les versions d’Exchange commençant par Exchange 2013. 
  
<sup>5</sup> ConvertId l’opération ne convertit pas correctement les identificateurs de dossier public à partir de l’identificateur EWS à l’identificateur de la banque. Vous pouvez mettre à jour manuellement l’identificateur qui est renvoyé sous la forme d’une [solution de contournement](http://msdn.microsoft.com/library/47d96cf6-9e2f-4fc0-9682-7258d3fbf918%28Office.15%29.aspx#bk_usingConvertId).
  
Les opérations suivantes ne sont pas pris en charge ou sont partiellement pris en charge, pour les dossiers publics dans les versions d’Exchange commençant par Exchange 2013 :
  
- **CopyFolder** (non pris en charge). Vous pouvez utiliser **CreateFolder** avec l’opération **CopyItems** pour implémenter la fonctionnalité d’opération **CopyFolder** . 
    
- **EmptyFolder** (non pris en charge). Vous pouvez utiliser **FindItem** avec l’opération **DeleteItem** pour implémenter la fonctionnalité d’opération **EmptyFolder** . 
    
- **MoveFolder** (partiellement pris en charge). Impossible de déplacer des dossiers entre des dossiers publics et privés. Vous pouvez déplacer des dossiers entre des dossiers publics et privés dans Exchange 2007 et Exchange 2010. Vous pouvez déplacer des dossiers dans un dossier public dans toutes les versions d’Exchange. 
    
EWS et l’API managée EWS ne prennent pas en charge les fonctionnalités suivantes pour les dossiers publics :
  
- À l’aide de **SyncFolderHierarchy**. Utilisez les opérations **FindFolder**, **GetFolder** et **SyncFolderItems** pour synchroniser des éléments et des dossiers dans une boîte aux lettres de dossier public. 
    
- Recherche-traversal profondeur de hiérarchie de dossiers publics. Utilisez **FindFolder** opération récursives à parcourir la hiérarchie de dossiers publics. 
    
- Utilisation de l’opération **CreateFolderPath** pour créer une hiérarchie de dossiers pour les dossiers publics. Vous devez utiliser l’opération **CreateFolder** pour chaque niveau de dossier dans une hiérarchie de dossiers distincts lorsque vous ciblez une boîte aux lettres de dossier public. 
    
- Enregistrer une copie des messages électroniques envoyés à l’aide de l’opération **CreateItem** . Au lieu de cela, utilisez l’opération **MoveItem** pour placer une copie du message dans un dossier public. 
    
## <a name="scenarios-for-using-ews-and-the-ews-managed-api-to-work-with-public-folders"></a>Scénarios d’utilisation EWS et l’API managée EWS pour travailler avec les dossiers publics
<a name="bk_scenarios"> </a>

Les dossiers publics permettent de nombreux scénarios importants pour les utilisateurs de boîte aux lettres Exchange. Vous pouvez permettre aux utilisateurs à l’aide de EWS et les API managées pour implémenter des solutions personnalisées pour l’accès et utilisation des dossiers publics et leur contenu. 
  
### <a name="programmatically-access-email-messages-that-have-been-sent-to-distribution-lists"></a>Par programme les e-mails access qui ont été envoyés aux listes de distribution

Les utilisateurs de boîte aux lettres Exchange peuvent utiliser des dossiers publics pour stocker des messages électroniques qui sont envoyés à des listes de distribution. Il s’agit d’un moyen pratique d’enregistrer l’historique de liste de distribution. Vous pouvez utiliser l' [opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) dans EWS ou les méthodes **ExchangeService.FindItems()** et **Folder.FindItems()** dans l’API managée EWS pour accéder aux messages électroniques de liste distribution stockée. 
  
### <a name="share-important-email-messages-and-other-mailbox-items"></a>Partager des messages électroniques importants et autres éléments de boîte aux lettres

Les utilisateurs de boîte aux lettres peuvent utiliser des dossiers publics comme référentiel partagé pour les éléments de boîte aux lettres. Différents utilisateurs d’une organisation peuvent partager des messages électroniques importants ou des contacts à l’aide de dossiers publics. EWS peut fournir l’accès à ces éléments de boîte aux lettres partagée. Vous pouvez utiliser l' [opération MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) dans EWS ou la méthode **Item.Move()** dans l’API managée EWS pour déplacer des messages électroniques, contacts et autres éléments de boîte aux lettres connecter et se déconnecter d’un dossier public. 
  
### <a name="public-discussions-with-post-items"></a>Discussions publiques avec des éléments de publication

Les dossiers publics sont un conteneur pratique pour les éléments de publication. Éléments de publications permettent d’utiliser des thèmes de conversation sans avoir à envoyer des messages électroniques entre les utilisateurs. Les utilisateurs peuvent utiliser des dossiers publics et publier des éléments pour héberger et gérer des thèmes de conversation entre les utilisateurs de boîtes aux lettres différente dans une organisation. De cette manière, les utilisateurs de boîte aux lettres peuvent accéder à l’historique de la conversation qu’utilise publier des éléments même si elles ne sont pas partie de la conversation partagé. Vous pouvez utiliser l' [opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) dans EWS ou la méthode **Item.Save()** dans l’API managée EWS pour créer et répondre afin de publier les éléments stockés dans un dossier public. 
  
## <a name="routing-public-folder-requests"></a>Routage des demandes de dossier public
<a name="bk_routing"> </a>

Contenu des dossiers publics peut être stocké sur plusieurs serveurs de boîtes aux lettres. La hiérarchie de dossiers publics peut être stockée sur une boîte aux lettres, tandis que le contenu du dossier public est stocké sur un autre. Et chacun de ces serveurs peut être différent du serveur de boîtes aux lettres de l’utilisateur demandant les informations. Dans ce cas, il est important d’inclure les en-têtes X-AnchorMailbox et X-PublicFolderMailbox supplémentaires dans vos requêtes de dossier public pour recevoir des informations précises sur les dossiers publics.
  
La valeur pour les AnchorMailbox X X-PublicFolderMailbox peut être différente selon si vous effectuez une demande de lié à la hiérarchie de dossiers ou le contenu du dossier. Le tableau suivant présente la procédure à suivre pour chaque méthode d’API managées ou l’opération EWS.
  
**Méthodes d’API managées et opérations EWS pour le routage des demandes de dossier public**

|**Lors de l’appel de ces méthodes.**|**Lors de l’appel de ces opérations**|**Utilisez cette procédure**|
|:-----|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |Routage des demandes de hiérarchie de dossiers publics  <br/> |
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |Routage des demandes de contenu de dossier public  <br/> |
   
## <a name="version-differences"></a>Différences entre les versions
<a name="VersionDifferences"> </a>

Dans Exchange 2007 et Exchange 2010, l’opération **ConvertId** fonctionne comme prévu lors de la conversion des identificateurs de dossier public à partir de l’identificateur EWS à l’identificateur de la banque. 
  
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Limites de dossiers publics](http://technet.microsoft.com/en-us/library/dn594582%28v=exchg.150%29.aspx)
    
- [FAQ : Dossiers publics](http://technet.microsoft.com/en-us/library/jj552408.aspx)
    
- [Procédures de dossier public](http://technet.microsoft.com/en-us/library/jj657481.aspx)
    

