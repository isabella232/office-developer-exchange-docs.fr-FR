---
title: Paramètres de l'application persistant dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: Découvrez les différentes options que votre API gérée EWS ou votre application EWS peut utiliser pour créer des paramètres d’application personnalisée persistants dans Exchange.
ms.openlocfilehash: 3fdc7ad3d5acabf6b498743afe8d93f0eff048c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516137"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Paramètres de l'application persistant dans EWS dans Exchange

Découvrez les différentes options que votre API gérée EWS ou votre application EWS peut utiliser pour créer des paramètres d’application personnalisée persistants dans Exchange.
  

  
Le moyen le plus simple de maintenir la synchronisation des configurations client personnalisées pour une boîte aux lettres, ou des dossiers et des éléments dans une boîte aux lettres, consiste à stocker les paramètres d’application sur un serveur Exchange serveur. Vous pouvez vous assurer que ces paramètres sont persistants pour une boîte aux lettres à l’aide de l’une des façons suivantes : 
  
- Objets de configuration utilisateur
    
- Propriétés étendues
    
- Éléments personnalisés
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>Quelles sont mes options pour créer des paramètres d’application persistants ?
<a name="Options"> </a>

Les objets de configuration utilisateur sont la meilleure option pour stocker les paramètres de configuration de vos applications clientes EWS. Vous pouvez également utiliser des propriétés étendues ou des éléments personnalisés, ou une combinaison des trois. Choisissez votre option en fonction de l’étendue de vos paramètres et selon que vos paramètres doivent être disponibles pour d’autres applications.
  
**Tableau 1. Options recommandées pour la création de paramètres d’application persistants en fonction de l’étendue**

|**Définition de l’étendue**|**Utilisez...**|**Accès par**|
|:-----|:-----|:-----|
|Item  <br/> |Propriété étendue sur un élément existant.  <br/> |Toute application EWS. Seuls les clients EWS qui connaissent l’identificateur de propriété peuvent accéder à une propriété étendue.  <br/> |
|Folder  <br/> |Objet de configuration utilisateur sur le dossier cible. Il s’agit d’un bon moyen d’enregistrer les paramètres d’affichage d’un dossier.  <br/> |Toute application EWS.  <br/> |
|Boîte aux lettres  <br/> |Objet de configuration utilisateur dans le dossier msgrootfolder par défaut.  <br/> |Toute application EWS.  <br/> |
   
### <a name="user-configuration-objects"></a>Objets de configuration utilisateur
<a name="UserConfig"> </a>

Les objets de configuration utilisateur sont des éléments spéciaux associés à des dossiers dans une boîte aux lettres. Les objets de configuration utilisateur, également appelés éléments associés à un dossier, sont généralement la meilleure option pour la persistance des paramètres d’application, en particulier si les informations de configuration sont associées à un dossier ou à une boîte aux lettres. En règle générale, ils ne sont pas indiqués aux utilisateurs finaux. Étant donné qu’ils peuvent stocker en natif des flux de données et des dictionnaires de données, ils sont parfaits pour stocker les informations de configuration. La meilleure façon d’utiliser des objets de configuration utilisateur consiste à stocker un ensemble de configurations dans un document XML, puis à enregistrer ces informations dans l’une des propriétés de flux de configuration utilisateur.
  
Les objets de configuration utilisateur sont accessibles différemment des autres types d’éléments stockés dans une boîte aux lettres. Vous pouvez utiliser la méthode d’API gérée EWS [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) ou l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS pour rechercher tous les éléments, mais vous devez utiliser l’option de traversée de recherche associée pour rechercher des objets de configuration utilisateur.  La **traversée de** recherche associée indique que les résultats de la recherche doivent contenir uniquement des objets de configuration utilisateur. EWS inclut un ensemble d’opérations spécifiques aux objets de configuration utilisateur. 
  
**Tableau 1. Opérations EWS et méthodes d’API gérées EWS pour l’utilisation des objets de configuration utilisateur**

|**Afin de...**|**Utiliser cette opération EWS**|**Utiliser cette méthode d’API gérée EWS**|
|:-----|:-----|:-----|
|Créer un objet de configuration utilisateur  <br/> |[Opération CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[UserConfiguration.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|Obtenir un objet de configuration utilisateur  <br/> |[Opération GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[UserConfiguration.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [UserConfiguration.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|Mettre à jour un objet de configuration utilisateur  <br/> |[Opération UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[UserConfiguration.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|Supprimer un objet de configuration utilisateur  <br/> |[Opération DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> Les objets de configuration utilisateur créés à l’aide d’EWS ont un [préfixe ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) qui commence par « IPM ». Configuration. ». ItemClass **d’un** objet de configuration utilisateur est le préfixe de l’objet de configuration utilisateur et le nom de l’objet de configuration utilisateur. Vous pouvez utiliser la propriété [Item.ItemClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API ou l’élément EWS **ItemClass** pour rechercher des objets de configuration utilisateur que vous avez définis. 
  
### <a name="extended-properties"></a>Propriétés étendues
<a name="ExtendedProperties"> </a>

Utilisez [les propriétés étendues](properties-and-extended-properties-in-ews-in-exchange.md) si vous souhaitez stocker des informations de configuration sur des éléments. EWS, contrairement à MAPI, ne retourne pas de sac de propriétés pour les éléments. Cela signifie qu’un client EWS doit connaître l’identificateur de propriété étendue pour rechercher et accéder à la propriété étendue. Si vous devez stocker des informations de configuration sur des éléments autres que des objets de configuration utilisateur, l’utilisation de propriétés étendues pour créer des propriétés personnalisées peut être la solution pour vous. Les propriétés étendues vous permettent d’accéder et de stocker des informations sur les propriétés qui ne font pas partie du jeu de propriétés standard d’un élément. 
  
> [!IMPORTANT]
> Le Exchange base de données de données contient un nombre fini de propriétés. Le nombre maximal d’identificateurs de propriétés pour Exchange base de données est de 32 767. Si vous utilisez des propriétés étendues pour stocker de nombreux paramètres, nous vous suggérons d’utiliser une seule propriété étendue pour stocker ces paramètres afin de ne pas dépasser ce maximum. 
  
Vous pouvez utiliser la méthode [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) EWS Managed API ou l’opération [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS pour définir des propriétés étendues sur les objets de configuration utilisateur. 
  
### <a name="custom-items"></a>Éléments personnalisés
<a name="CustomItems"> </a>

Les éléments personnalisés peuvent également être utilisés pour stocker des informations. Les propriétés d’élément existantes peuvent être réaffectées pour contenir des informations de configuration. Vous pouvez également utiliser des propriétés étendues pour définir vos propres propriétés pour votre application. L’utilisation d’éléments personnalisés pour stocker la configuration offre les avantages suivants : 
  
- Elles fonctionnent pour toutes les versions de Exchange prise en charge d’EWS.
    
- Si vous n’utilisez pas de propriétés étendues sur l’élément, le budget de Exchange propriétés n’est pas facturé.
    
## <a name="where-should-i-store-my-application-settings"></a>Où dois-je stocker mes paramètres d’application ?
<a name="ApplicationSettingsLocation"> </a>

Les dossiers de boîte aux lettres et les éléments qu’ils contient se trouvent dans le dossier de message racine. Ce dossier est identifié par la valeur [WellKnownFolderName.msgfolderroot](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) dans l’API gérée EWS. En termes MAPI, il s’agit de l’équivalent de la sous-arbre IPM d’une boîte aux lettres. Les objets de configuration utilisateur sont souvent utilisés pour créer des paramètres basés sur l’interface utilisateur, afin qu’une application puisse afficher les paramètres d’affichage en fonction du dossier accessible par un utilisateur. Les paramètres d’affichage basé sur un dossier sont généralement définies sur un objet de configuration utilisateur associé au dossier. Mais parfois, vous souhaitez peut-être rendre vos paramètres globaux pour votre application. Dans ce cas, vous pouvez stocker vos paramètres dans le dossier de message racine. 
  
La plupart des utilisateurs ne connaissent pas le dossier de boîte aux lettres racine et n’y accèdent généralement pas. Ce dossier est identifié par la [valeur WellKnownFolderName.root](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) dans l’API gérée EWS. En termes MAPI, il s’agit de l’équivalent de la sous-arbre non IPM d’une boîte aux lettres. Les informations que les utilisateurs finaux n’accèdent pas directement sont stockées dans le dossier de boîte aux lettres racine. Vous pouvez stocker le paramètre de votre application dans ce dossier, car les applications clientes n’y accèdent généralement pas. 
  
## <a name="version-differences"></a>Différences entre les versions
<a name="VersionDifferences"> </a>

Les objets de configuration utilisateur sont disponibles sur Exchange Online, Exchange Online dans le cadre de Office 365 et les versions de Exchange à partir de Exchange 2010.
  
## <a name="see-also"></a>Voir aussi


- [Gérer les paramètres d’application persistants à l’aide d’EWS dans Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Utiliser des dossiers à l’aide d’EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Utilisations d’éléments de boîte aux lettres Exchange à l’aide d’EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

