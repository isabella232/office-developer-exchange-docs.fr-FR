---
title: Vue d'ensemble de la conception client EWS pour Exchange
manager: sethgros
ms.date: 3/11/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: b26f67aa-7c66-4d7d-98b3-746f26ab37f4
description: Découvrez les considérations de conception pour le développement avec EWS pour Exchange.
ms.openlocfilehash: ea0e1ad3f8402d19a6163f3320a2a17f08f3ea2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754779"
---
# <a name="ews-client-design-overview-for-exchange"></a>Vue d'ensemble de la conception client EWS pour Exchange

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. Découvrez les considérations de conception pour le développement avec EWS pour Exchange. 
  
Cet article fournit des informations générales sur la conception d'une application Exchange Web Services (EWS). Vous pouvez utiliser ces informations pour déterminer si EWS représente une API appropriée pour votre application, et si c'est le cas, quel type de mise en œuvre du client vous devez utiliser. Cet article fournit également des informations sur les meilleures pratiques en matière de conception d'applications pouvant cibler Office 365, Exchange Online et les versions d'Exchange depuis Exchange 2007, dans une base de code, ainsi que d'importants points permettant de faire un choix entre le ciblage de serveurs Exchange locaux et le ciblage d'Exchange Online.
  
## <a name="is-ews-the-right-api-for-your-application"></a>EWS représente-t-il une API appropriée pour votre application ?
<a name="IsEWSRight"> </a>

Avant de commencer à concevoir votre application, il est important de déterminer si EWS représente l'API appropriée pour vous. Si vous développez à l'aide d'Exchange Server ou d'Exchange Online, EWS est la technologie d'accès au client privilégiée. Le développement d'accès au client pour les versions d'Exchange 0 partir d'Exchange 2007 s'est principalement concentré sur EWS. La nouvelle fonctionnalité d'accès au client implémentée dans Outlook utilise EWS, y compris les fonctionnalités Absent(e) du bureau et Disponible introduites dans Exchange 2007, et les fonctionnalités Infos-courrier et Obtenir des salles introduites dans Exchange 2010. Cela représente un investissement engagé dans EWS pour les partenaires internes et externes qui développent des applications clientes Exchange.
  
EWS est l'API d'accès au client principale pour vos applications clientes Exchange. Toutefois, dans certains cas, vous pouvez envisager d'utiliser d'autres API Exchange pour le développement d'applications clientes. Par exemple, Exchange ActiveSync offre les avantages suivants, contrairement à EWS :
  
- La structure XML a été tokenisée pour transformer Exchange ActiveSync en un protocole plus compact.  
- ActiveSync Exchange contient un mécanisme de stratégie pour contrôler l'accès au client et fournir d'autres solutions de messagerie mobile d'entreprise robustes.
    
> [!NOTE]
> [!REMARQUE] Vous avez besoin d'une licence pour développer des clients Exchange ActiveSync. Pour en savoir plus sur les différences entre Exchange ActiveSync et EWS, voir [Choisir entre Exchange ActiveSync et Exchange Web Services (EWS)](http://msdn.microsoft.com/en-us/library/dn144954%28v=exchg.140%29.aspx). 
  
RPC MAPI sur HTTP est une autre option de programmabilité pour les applications clientes Exchange. Toutefois, RPC MAPI sur HTTP ne fournit pas d'interface intuitive pour la communication entre les clients et le serveur.
  
Pour plus d’informations sur les technologies de développement Exchange, voir [Explorer l’API managée EWS, EWS et des services web Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).
  
## <a name="options-for-ews-client-development"></a>Options pour le développement de clients EWS
<a name="EWSClientOptions"> </a>

Plusieurs options sont disponibles pour le développement sur Exchange à l'aide d'EWS. La meilleure option dépend de la plateforme de développement, des outils, des implémentations disponibles et des exigences en matière d'application pour votre organisation. Les quatre options principales disponibles pour la création d'applications clientes EWS sont les suivantes :
  
- API managée EWS
- API Java EWS
- Proxys générés automatiquement EWS
- API cliente EWS personnalisée
    
### <a name="ews-managed-api"></a>API managée EWS

L'[API managée EWS](http://aka.ms/ews-managed-api-readme) est un client de service web personnalisé. Il s'agit de l'API d'accès au client standard pour les applications .NET Framework. 
  
Voici quelques-uns des avantages que représente l'utilisation de l'API managée EWS :
  
- elle fournit un modèle objet intuitif ;   
- elle résume les complexités de la description de service dans les fichiers WSDL et de schéma ;   
- elle comprend une logique métier côté client ;   
- elle gère les requêtes et réponses web, ainsi que la sérialisation et désérialisation d'objet ;   
- elle est prise en charge par Microsoft.
    
Notez toutefois que l'API managée EWS n'est pas une solution complète. Certaines fonctionnalités ne sont pas implémentées dans l'API managée EWS. Bien qu'elle n'implémente pas toutes les fonctionnalités EWS, elle peut représenter le meilleur choix pour votre développement d'application cliente, pour les raisons suivantes :
  
- vous pouvez utiliser .NET Framework pour le développement ;
- elle implémente la découverte automatique en plus de la plupart des parties du modèle objet EWS ;
- elle implémente la logique métier côté client pour l'utilisation d'EWS, dans la classe [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). 
    
Vous pouvez choisir d'utiliser l'API de service web EWS au lieu de l'API managée EWS pour les raisons suivantes :
  
- votre application n'utilise pas .NET Framework ; 
- vous ne voulez pas distribuer l'assembly d'API managée EWS ; 
- votre application utilise des fonctionnalités qui ne sont pas implémentées dans l'API managée EWS.
    
Pour plus d'informations, voir [Prise en main des applications clientes d'API managée EWS](get-started-with-ews-managed-api-client-applications.md).
  
> [!NOTE]
> L’API managée EWS est désormais disponible sous forme d’un projet open source sur les [référentiels](http://aka.ms/ews-managed-api-github). Vous pouvez utiliser la bibliothèque open source pour : 
> - participer aux résolutions de bogues et aux améliorations apportées à l’API ; 
> - obtenir des correctifs et des améliorations avant qu’ils soient disponibles dans une version officielle ;
> - accéder à l’implémentation la plus complète et la plus à jour de l’API, afin de l’utiliser comme référence ou pour créer des bibliothèques sur de nouvelles plateformes.
> 
> Vos [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via référentiels sont les bienvenus. 
  
### <a name="ews-java-api"></a>API Java EWS

L'API Java EWS est un projet open source sur [GitHub](https://github.com/OfficeDev/ews-java-api) qui peut être mis à jour et étendu par la communauté. Elle est stylistiquement semblable à l' [API managée EWS](http://msdn.microsoft.com/en-us/library/office/jj220535%28v=exchg.80%29.aspx) et utilise les requêtes et réponses SOAP EWS sur le réseau. Bien que vous ne puissiez pas accéder à toutes les [opérations SOAP EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) à l'aide de l'API Java EWS, avec la [création récente](http://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/) du projet open source, nous attendons que la communauté comble cette lacune. Notez que le support Microsoft, avec un contrat de support approprié, traite les questions relatives au protocole SOAP EWS, mais pas à l'API Java EWS. Cette dernière est disponible pour téléchargement et pour contribution de la communauté sur [GitHub](https://github.com/OfficeDev/ews-java-api).
  
### <a name="ews-autogenerated-proxies"></a>Proxys EWS générés automatiquement

Les API clientes générées automatiquement sont générées à partir de WSDL EWS et de définitions de schéma XML. Les générateurs de modèle objet client sont disponibles dans de nombreuses langues. En règle générale, les modèles objet générés automatiquement gèrent la sérialisation et désérialisation d'objet. Ils n'incluent pas de logique métier et le processus de génération automatique crée souvent des artefacts qui rendent le modèle objet moins intuitif lors de l'utilisation. Le support Exchange prend en charge le code XML qui est envoyé et reçu par le client, mais pas le modèle objet.
  
### <a name="custom-ews-client-api"></a>API cliente EWS personnalisée

Pour certaines applications qui utilisent un petit ensemble de fonctionnalités EWS, vous pouvez créer une API cliente personnalisée pour communiquer avec Exchange et afin d'utiliser moins de ressources système. Cela est utile pour les clients qui s'exécutent sur des périphériques limités par la mémoire, tels que les clients exécutant .NET Micro Framework.
  
## <a name="ews-client-features"></a>Fonctionnalités clientes EWS
<a name="EWSFeatures"> </a>

Quelle que soit l'option de développement que vous choisissez, vous devez penser à la façon dont les fonctionnalités EWS sont implémentées dans votre client. La disponibilité des fonctionnalités est basée sur la version du schéma EWS ciblée par votre application. Étant donné que les schémas EWS sont compatibles en amont et en aval, si vous créez une application qui cible une version de schéma antérieure, comme Exchange Server 2007 SP1, votre application fonctionnera également sur une version de schéma ultérieure, comme le service Exchange Server 2013 SP1, ainsi qu'Exchange Online. 
  
Étant donné que les fonctionnalités et les mises à jour de fonctionnalité sont pilotées par le schéma, nous vous recommandons d'utiliser la base de code commun la plus récente ciblant les fonctionnalités EWS que vous souhaitez mettre en œuvre dans votre application cliente. De nombreuses applications peuvent cibler la version Exchange2007_SP1, car le schéma Exchange 2007 SP1 contient presque toutes les principales fonctionnalités Exchange pour travailler avec des éléments et des dossiers dans la banque d'informations Exchange. Il est recommandé de conserver des branches de code pour chaque version de schéma EWS. Vous trouverez ci-dessous les versions de schéma actuellement disponibles. 
  
```XML
  <xs:simpleType name="ExchangeVersionType">
    <xs:restriction base="xs:string">
      <xs:enumeration value="Exchange2007" />
      <xs:enumeration value="Exchange2007_SP1" />
      <xs:enumeration value="Exchange2010" />
      <xs:enumeration value="Exchange2010_SP1" />
      <xs:enumeration value="Exchange2010_SP2" />
      <xs:enumeration value="Exchange2013" />
      <xs:enumeration value="Exchange2013_SP1" />
    </xs:restriction>
  </xs:simpleType>
```

Les versions de schéma sont conservées dans le type simple **ExchangeVersionType**. 
  
Pour plus d'informations sur les fonctionnalités disponibles dans chaque version de schéma EWS, voir [Versions de schéma EWS dans Exchange](ews-schema-versions-in-exchange.md).
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Disponibilité des fonctionnalités Web service API dans Exchange et de l'API managée EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
    
- [Versions de schéma EWS dans Exchange](ews-schema-versions-in-exchange.md)
    
- [Options de configuration pour EWS dans Exchange](configuration-options-for-ews-in-exchange.md)
    
- [Comparaison d'Exchange Online et programmation du client Exchange sur site](comparing-exchange-online-and-exchange-on-premises-client-programming.md)
    
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    
- [Besoins de redistribution pour l'API managée EWS](redistribution-requirements-for-the-ews-managed-api.md)
    
- [L'instrumentation des demandes du client pour EWS et reste dans Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi
 
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md) 
- [Types d'applications EWS](ews-application-types.md)
    

