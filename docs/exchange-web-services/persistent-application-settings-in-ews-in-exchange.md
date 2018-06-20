---
title: Paramètres d’application persistants dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 394d4e70-8517-4073-809a-5b61780ff923
description: En savoir plus sur les différentes options que votre API managées ou les applications EWS permet de créer des paramètres d’application personnalisés persistent dans Exchange.
ms.openlocfilehash: b384fd5608dc647950d7cd31e861e24c12e3316f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755063"
---
# <a name="persistent-application-settings-in-ews-in-exchange"></a>Paramètres d’application persistants dans EWS dans Exchange

En savoir plus sur les différentes options que votre API managées ou les applications EWS permet de créer des paramètres d’application personnalisés persistent dans Exchange.
  

  
Pour synchroniser les configurations du client personnalisé pour une boîte aux lettres, ou des dossiers et des éléments dans une boîte aux lettres, le plus simple consiste à stocker les paramètres de l’application sur un serveur Exchange. Vous pouvez vous assurer que ces paramètres conserver pour une boîte aux lettres à l’aide d’une des options suivantes : 
  
- Objets de configuration utilisateur
    
- Propriétés étendues
    
- Autres éléments personnalisés
    
## <a name="what-are-my-options-for-creating-persistent-application-settings"></a>Quelles sont mes options pour la création de paramètres d’application persistants ?
<a name="Options"> </a>

Objets de configuration utilisateur sont votre meilleure option pour stocker les paramètres de configuration pour vos applications de client EWS. Vous pouvez également utiliser étendre les propriétés ou autres éléments personnalisés ou une combinaison des trois. Choisissez l’option en fonction de l’étendue de vos paramètres et si vos paramètres doivent être disponibles à d’autres applications.
  
**Le tableau 1. Options recommandées pour la création de paramètres d’application persistant en fonction de l’étendue**

|**Définition de l’étendue**|**Utilisez...**|**Accessible par**|
|:-----|:-----|:-----|
|Élément  <br/> |Une propriété étendue sur un élément existant.  <br/> |N’importe quelle application EWS. Seuls les clients EWS connaître l’identificateur de la propriété peuvent accéder à une propriété étendue.  <br/> |
|Folder  <br/> |Un objet de configuration utilisateur sur le dossier cible. Il s’agit d’un bon moyen pour enregistrer les paramètres d’affichage d’un dossier.  <br/> |N’importe quelle application EWS.  <br/> |
|Boîte aux lettres  <br/> |Un objet de configuration utilisateur dans le dossier msgrootfolder par défaut.  <br/> |N’importe quelle application EWS.  <br/> |
   
### <a name="user-configuration-objects"></a>Objets de configuration utilisateur
<a name="UserConfig"> </a>

Objets de configuration utilisateur sont des éléments spéciaux qui sont associés à des dossiers dans une boîte aux lettres. Objets de configuration utilisateur, également appelés éléments d’un dossier associé, sont généralement la meilleure option pour les paramètres d’application persistantes, notamment si les informations de configuration soient associées à un dossier ou d’une boîte aux lettres. Ils sont généralement pas exposées aux utilisateurs finaux. Car ils peuvent stocker en mode natif des dictionnaires de données et de flux de données, ils sont idéales pour stocker les informations de configuration. La meilleure façon d’utiliser des objets de configuration utilisateur consiste à stocker un ensemble de configurations dans un document XML, puis enregistrez ces informations dans une des propriétés de flux de données de configuration utilisateur.
  
Accès à des objets de configuration utilisateur différemment des autres types d’éléments stockés dans une boîte aux lettres. Vous pouvez utiliser la méthode d’API managées [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=EXCHG.80%29.aspx) ou l’opération EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher tous les éléments, mais vous devez utiliser l’option de traversée de recherche **associé** pour rechercher des objets de configuration utilisateur. Le parcours de recherche **associé** indique que les résultats de recherche doivent contenir uniquement des objets de configuration utilisateur. EWS inclut un ensemble d’opérations qui sont spécifiques aux objets de configuration utilisateur. 
  
**Le tableau 1. Opérations EWS et méthodes d’API managées pour travailler avec les objets de configuration utilisateur**

|**Pour...**|**Utilisez cette opération EWS**|**Utilisez cette méthode de l’API managée EWS**|
|:-----|:-----|:-----|
|Créer un objet de configuration utilisateur  <br/> |[Opération CreateUserConfiguration](http://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) <br/> |[UserConfiguration.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) <br/> |
|Obtenir un objet de configuration utilisateur  <br/> |[Opération GetUserConfiguration](http://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |[UserConfiguration.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> [UserConfiguration.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.load%28v=exchg.80%29.aspx) <br/> |
|Mettre à jour un objet de configuration utilisateur  <br/> |[Opération UpdateUserConfiguration](http://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) <br/> |[UserConfiguration.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) <br/> |
|Supprimer un objet de configuration utilisateur  <br/> |[Opération DeleteUserConfiguration](http://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) <br/> |[UserConfiguration.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) <br/> |
   
> [!NOTE]
> Les objets de configuration utilisateur créés à l’aide de EWS ont un préfixe [ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) qui commence par « IPM. Configuration. ». **ItemClass** d’un objet de configuration utilisateur est le préfixe d’objet de configuration utilisateur et votre nom d’objet de configuration utilisateur. Vous pouvez utiliser la propriété d’API managées [Item.ItemClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) ou l’élément **ItemClass** EWS pour rechercher des objets de configuration d’utilisateur que vous avez définis. 
  
### <a name="extended-properties"></a>Propriétés étendues
<a name="ExtendedProperties"> </a>

Utilisez les [Propriétés étendues](properties-and-extended-properties-in-ews-in-exchange.md) si vous souhaitez stocker les informations de configuration sur les éléments. EWS, contrairement à MAPI, ne renvoie pas un conteneur des propriétés des éléments. Cela signifie qu’un client EWS doit connaître l’identificateur de la propriété étendue afin de trouver et accéder à la propriété étendue. Si vous avez besoin stocker les informations de configuration sur les éléments autres que des objets de configuration utilisateur, à l’aide des propriétés étendues pour créer des propriétés personnalisées peut-être être la solution pour vous. Les propriétés étendues permettent d’accéder et stocker des informations sur les propriétés qui ne font pas partie de la propriété standard est définie pour un élément. 
  
> [!IMPORTANT]
> Le schéma de base de données Exchange a un nombre limité de propriétés. Le nombre maximal d’identificateurs de propriété pour une base de données Exchange est 32 767. Si vous utilisez les propriétés étendues pour stocker de nombreux paramètres, nous vous suggérons d’utiliser une seule propriété étendue pour stocker ces paramètres afin de ne pas dépasser ce maximum. 
  
Vous pouvez utiliser la méthode d’API managées [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=EXCHG.80%29.aspx) ou l’opération EWS [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) pour définir des propriétés étendues sur les objets de configuration utilisateur. 
  
### <a name="custom-items"></a>Autres éléments personnalisés
<a name="CustomItems"> </a>

Autres éléments personnalisés peuvent également servir à stocker les informations. Les propriétés d’élément existant peuvent être réaffectées contenant des informations de configuration. Ou bien, vous pouvez utiliser les propriétés étendues pour définir vos propres propriétés de votre application. À l’aide d’autres éléments personnalisés pour stocker la configuration offre les avantages suivants : 
  
- Ils fonctionnent pour toutes les versions d’Exchange qui prennent en charge EWS.
    
- Si vous n’utilisez pas les propriétés étendues sur l’élément, le propriétés Exchange pas facturation du budget.
    
## <a name="where-should-i-store-my-application-settings"></a>Où dois-je stocker les paramètres de mon application ?
<a name="ApplicationSettingsLocation"> </a>

Des éléments dans les dossiers boîte aux lettres se trouvent dans le dossier de message racine. Ce dossier est identifié par la valeur [WellKnownFolderName.msgfolderroot](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) dans l’API managée EWS. En termes MAPI, il s’agit de l’équivalent de la sous-arborescence IPM d’une boîte aux lettres. Objets de configuration utilisateur sont souvent utilisés pour créer des paramètres de l’interface utilisateur, afin qu’une application peut rendre des paramètres d’affichage basés sur le dossier qui accède à un utilisateur. Un affichage basé sur le dossier paramètres sont généralement définis sur un objet de configuration d’utilisateur qui est associé au dossier. Mais vous souhaiterez parfois, vérifiez vos paramètres globaux à votre application. Dans ce cas, vous pouvez stocker vos paramètres dans le dossier de message racine. 
  
La plupart des utilisateurs ne sont pas conscients d’et généralement n’accédez pas au dossier racine de boîte aux lettres. Ce dossier est identifié par la valeur [WellKnownFolderName.root](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) dans l’API managée EWS. En termes MAPI, il s’agit de l’équivalent de la sous-arborescence non-IPM d’une boîte aux lettres. Les informations que les utilisateurs finaux ne pas y accéder directement sont stockées dans le dossier racine de boîte aux lettres. Vous souhaitez stocker votre paramètre d’application dans ce dossier, car les applications client n’accèdent pas généralement il. 
  
## <a name="version-differences"></a>Différences entre les versions
<a name="VersionDifferences"> </a>

Objets de configuration utilisateur sont disponibles dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2010.
  
## <a name="see-also"></a>Voir aussi


- [Gérer les paramètres de l’application permanente à l’aide de EWS dans Exchange](how-to-manage-persistent-application-settings-by-using-ews-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    
- [Les propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Utilisation de dossiers à l’aide de EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)
    

