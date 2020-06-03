---
title: Versions de schéma EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d1ab6f9c-ea91-4022-830d-7f7b759e3935
description: Découvrez le schéma EWS et comment concevoir votre application pour qu’elle fonctionne avec elle, ainsi que les fonctionnalités disponibles avec chaque version de schéma et la façon dont le schéma est lié à la version du service Exchange.
localization_priority: Priority
ms.openlocfilehash: 6afef658e747b11d9aa5fb7d7a88ba8f5c57ac82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456011"
---
# <a name="ews-schema-versions-in-exchange"></a>Versions de schéma EWS dans Exchange

Découvrez le schéma EWS et comment concevoir votre application pour qu’elle fonctionne avec elle, ainsi que les fonctionnalités disponibles avec chaque version de schéma et la façon dont le schéma est lié à la version du service Exchange.
  
Le schéma EWS définit les structures de données qui peuvent être envoyées et renvoyées par Exchange. Chaque nouvelle version d’Exchange qui contient une modification importante apportée à la fonctionnalité EWS contiendra un nouveau schéma. EWS et le schéma EWS sont à la fois inverses et, dans certains cas, le transfert compatible-les applications conçues avec des versions antérieures d’EWS fonctionnent, dans la plupart des cas, avec les versions ultérieures d’EWS, et les applications qui ciblent les versions ultérieures d’EWS fonctionnent si les mêmes fonctionnalités étaient incluses dans une version antérieure. Cet article vous aidera à comprendre le rôle du schéma EWS, le fonctionnement des versions de schéma, la relation entre la version de schéma et la version de service, et comment concevoir votre application pour qu’elle fonctionne avec le schéma EWS. 
  
## <a name="role-of-the-ews-schema"></a>Rôle du schéma EWS

Le schéma EWS effectue les opérations suivantes :
  
- Définit l’ensemble de fonctionnalités disponibles pour un client. Un client peut obtenir la liste des versions de schéma prises en charge à l’aide du [service de découverte automatique](autodiscover-for-exchange.md)SOAP. Le client peut ensuite déterminer les fonctionnalités auxquelles il peut accéder, car chaque version de schéma représente un [jeu de fonctionnalités EWS](ews-schema-versions-in-exchange.md#bk_features). Chaque nouveau schéma publié pour EWS contient les entités de schéma de la version précédente, ainsi que les définitions de schéma de toutes les nouvelles fonctionnalités. De cette manière, EWS prend en charge les applications qui ciblent une version antérieure d’EWS.
    
- Fournit une description générale du contrat d’API. Vous pouvez utiliser ce contrat pour déterminer les structures de données qui peuvent être envoyées et reçues à partir d’Exchange.
    
- Fournit un mécanisme de gestion des versions pour l’envoi de demandes. Le serveur Exchange contient toutes les versions de schéma EWS prises en charge dans son répertoire virtuel. 
    
## <a name="designing-your-application-with-schema-version-in-mind"></a>Conception de votre application avec la version de schéma à l’esprit

Gardez les points suivants à l’esprit lors de la conception de votre application de sorte qu’elle fonctionne avec différentes versions du schéma EWS :
  
- Activer/désactiver la fonctionnalité en fonction de la version du schéma. Vous pouvez mapper les fonctionnalités du client à la version de schéma et, dans certains cas, à la version du service. L’exemple suivant renverra un [PropertySet](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) basé sur la version du schéma et du service. 
    
  ```cs
  private static PropertySet InitPropertySetByVersion(ExchangeService service)
  {
      PropertySet props;
      // The schema version to target to access the NormalizedBody property 
      // is Exchange2013 or later. The server version to target to access the 
      // NormalizedBody property on an email is 15 or later, which 
      // equates to Exchange 2013.
      if (service.RequestedServerVersion >= ExchangeVersion.Exchange2013 &amp;&amp;
          service.ServerInfo.MajorVersion >= 15)
      {
          props = new PropertySet(EmailMessageSchema.NormalizedBody);
      }
      else
      {
          props = new PropertySet(EmailMessageSchema.Body);
      }
      return props;
  }
  ```

- Version de vos demandes avec la version la plus ancienne du schéma EWS qui prend en charge les fonctionnalités que vous souhaitez utiliser. Cela permettra à votre client de s’appliquer à un plus grand nombre de serveurs Exchange potentiels. Cette fonction est moins importante si vous développez une application métier pour cibler les serveurs de votre organisation uniquement, mais elle est très importante si vous créez une application pour une audience plus large.
    
## <a name="features-by-schema-version"></a>Fonctionnalités par version de schéma
<a name="bk_features"> </a>

Les versions de schéma disponibles pour un client sont identifiées dans le type simple **ExchangeVersionType** situé dans le schéma types. xsd. L' **ExchangeVersionType** est implémenté par l’élément [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) . L’élément **RequestServerVersion** est envoyé dans toutes les demandes EWS pour indiquer au serveur la version du schéma que le client cible. Cette option identifie à son tour l’ensemble de fonctionnalités disponibles pour le client. 
  
**Tableau 1 : fonctionnalités EWS par produit et version de schéma**

|**Version du produit**|**Version de schéma associée**|**Composants**|
|:-----|:-----|:-----|
|Exchange Online  |Version de schéma la plus récente.  |Inclut toutes les fonctionnalités de la version actuelle d’Exchange, ainsi que les nouvelles fonctionnalités ajoutées pour les clients en ligne. |
|Exchange 2013 SP1 |Exchange2013_SP1 | Inclut toutes les fonctionnalités d’Exchange 2013.<br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2013 SP1 : <ul><li>[Stratégie de blocage des boîtes aux lettres](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) </li><li> [Proposition d’un nouvel horaire](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) </li><li>  Mettre à jour les accusés de réception pour la [mise à jour](https://msdn.microsoft.com/library/office/dn600559%28v=exchg.80%29.aspx) et [la suppression](https://msdn.microsoft.com/library/office/dn600557%28v=exchg.80%29.aspx) des éléments  </li><li> Mise à jour des [informations IRM](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.conversation.hasirm%28v=exchg.80%29.aspx) pour les conversations  </li></ul> |
|Exchange 2013   |Exchange2013   | Inclut toutes les fonctionnalités introduites dans Exchange 2007 et Exchange 2010. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2013 :<ul><li>Archivage  </li><li>  eDiscovery  </li><li>  Personnages  </li><li>  Stratégies de rétention  </li><li>  Magasin de contacts unifié  </li><li>  Photos de l'utilisateur  </li></ul> |
|Exchange 2010 SP2   |Exchange2010_SP2 | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP1. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP2 :<ul><li>Obtenir l’expiration du mot de passe  </li><li>  DateTime, précision  </li><li>  Identificateurs de propriété mis à jour pour les contacts  </li><li>  Nouveaux scénarios d’usurpation d’identité  </li></ul> |
|Exchange 2010 SP1  |Exchange2010_SP1   | Inclut toutes les fonctionnalités introduites dans Exchange 2010. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP1 :<ul><li>Créer, récupérer et modifier des règles de boîte de réception  </li><li>  Accès par programme à la boîte aux lettres d’archivage  </li><li>  Actions de conversation  </li><li>  Notifications de traversée de pare-feu  </li><li>  Fonctionnalités d’administration améliorées  </li><li>  Prise en charge améliorée des versions mixtes  </li><li>  Prise en charge de la protection de la limitation  </li><li>  Contrôle de l’accès des applications à EWS  </li><li>  Prise en charge de l’authentification par certificat client  </li></ul> |
|Exchange 2010  |Exchange2010   | Inclut toutes les fonctionnalités introduites dans Exchange 2007 SP1. <br/><br/>Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2010 :<ul><li>Liste de distribution privée complète  </li><li>  Objets de configuration utilisateur  </li><li>  Éléments associés aux dossiers  </li><li>  Suivi des messages  </li><li>  Messagerie unifiée  </li><li>  Découverte automatique SOAP  </li><li>  Prise en charge améliorée des fuseaux horaires  </li><li>  Informations de disponibilité des ressources de la salle  </li><li>  Recherche indexée  </li><li>  Accès à la benne  </li><li>  Informations sur les infos-courrier  </li></ul> |
|Exchange 2007 SP1   |Exchange2007_SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2007. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2007 SP1 :<ul><li>Gestion des délégués  </li><li>  Autorisations d’accès aux dossiers  </li><li>  Dossiers publics  </li><li>  Publier des éléments  </li><li>  Conversion d’ID  </li></ul>|
|Exchange 2007  |Exchange2007 | Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2007 :<ul><li>Accès total aux éléments, aux dossiers et aux pièces jointes (créer, obtenir, mettre à jour, supprimer)  </li><li>  Disponibilité  </li><li>  Paramètres d’absence du Bureau  </li><li>  Notifications  </li><li>  Synchronisation  </li><li>  Résolution de noms  </li><li>  Expansion de liste de distribution (DL)  </li><li>  Rechercher  </li></ul> |
   
## <a name="relationship-between-the-ews-schema-and-the-service-version"></a>Relation entre le schéma EWS et la version de service
<a name="bk_features"> </a>

La version du schéma EWS est liée à la version du service EWS que le serveur exécute. Le modèle d’affectation de noms pour le schéma EWS est lié aux versions locales d’Exchange. Par exemple, la version initiale d’Exchange 2013 a une version de service de 15.00.0516.032 et le nom de schéma **Exchange2013**. Étant donné que le schéma a été mis à jour pour Exchange 2013, Exchange 2013 et Exchange Online avec une version de service d' 15.00.0516.032 et les versions ultérieures ont le même nom de version pour le schéma le plus récent. Dans les versions antérieures d’Exchange, le schéma EWS n’a pas été mis à jour avec des mises à jour cumulatives (précédemment appelés correctifs cumulatifs). Étant donné qu’Exchange est mis à jour plus fréquemment pour prendre en charge Exchange Online, les mises à jour cumulatives contiennent maintenant des mises à jour de schéma pour EWS. Les noms de fichier de schéma et le nom de version de schéma associé sont uniquement mis à jour avec les service packs ou les versions majeures d’Exchange en local.
  
Bien que le schéma EWS définisse le contrat, dans certains cas, la version de service est le seul moyen pour un client de déterminer la façon dont il est supposé interagir avec le service. Les modifications de comportement de service qui ne sont pas reflétées dans le schéma peuvent uniquement être déterminées par la version de service renvoyée dans toutes les réponses EWS. Par exemple, lorsque les [dossiers publics](public-folder-access-with-ews-in-exchange.md) ont été reconçus dans Exchange 2013, les opérations utilisées pour déplacer et copier des dossiers publics ont été modifiées. Si vous avez conçu un client pour copier des dossiers publics dans Exchange 2010, vous devez le mettre à jour pour qu’il utilise des opérations différentes afin d’obtenir le même résultat dans Exchange 2013. 
  
## <a name="how-the-ews-schema-is-updated"></a>Mise à jour du schéma EWS
<a name="bk_features"> </a>

Les serveurs Exchange exécutant des versions d’Exchange à partir d’Exchange 2007 incluent le schéma EWS dans le répertoire virtuel qui héberge le service EWS. La version actuelle du schéma est toujours représentée par les fichiers types. xsd et messages. xsd. La figure 1 montre comment le schéma messages. xsd est bifurque lorsqu’une nouvelle version du schéma est développée. Avant l’ajout de nouvelles fonctionnalités, une copie du schéma messages. xsd d’origine est incluse et renommée pour représenter la version précédente du schéma. Le fichier messages. xsd est ensuite mis à jour avec la description de service de la nouvelle version.
  
**Figure 1. Mise à jour du schéma EWS**

![Illustration de la mise à jour du schéma EWS. La dernière version du schéma est divisée et renommée afin de représenter la version précédente et le dernier nom de fichier représente la version actuelle.](media/Ex15_EWS_Schema_Update1.png)
  
Avant la mise à jour du schéma EWS pour une nouvelle version, la version actuelle du schéma est dupliquée et renommée à l’aide de la Convention suivante :
  
`<schemaname>-<majorserverversion><servicepack>.xsd`
  
Le nom du fichier d’origine représente alors le schéma le plus récent. Toutes les nouvelles fonctionnalités sont ajoutées au dernier schéma, à l’exception des mises à jour et des correctifs pour les versions antérieures du schéma. 
  
## <a name="see-also"></a>Voir aussi

- [Versions de schéma EWS dans Exchange](ews-schema-versions-in-exchange.md) 
- [Découverte automatique pour Exchange](autodiscover-for-exchange.md) 
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

