---
title: Versions de schéma EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d1ab6f9c-ea91-4022-830d-7f7b759e3935
description: Découvrez le EWS schéma et la conception de votre application pour fonctionner avec elle, ainsi que les fonctionnalités disponibles avec chaque version de schéma et comment le schéma est lié à la version du service Exchange.
ms.openlocfilehash: dd8e85547666ba0bf3a1a38775260268594f2a8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754786"
---
# <a name="ews-schema-versions-in-exchange"></a>Versions de schéma EWS dans Exchange

Découvrez le EWS schéma et la conception de votre application pour fonctionner avec elle, ainsi que les fonctionnalités disponibles avec chaque version de schéma et comment le schéma est lié à la version du service Exchange.
  
Le schéma EWS définit les structures de données pouvant être envoyés à et renvoyées par Exchange. Chaque nouvelle version d’Exchange qui contient une modification significative de fonctionnalité EWS contiendra un nouveau schéma. EWS et le schéma EWS sont en arrière et dans certains cas, une compatibilité ascendante - applications conçues avec des versions antérieures de EWS fonctionne, dans la plupart des cas, avec les versions ultérieures de EWS, et les applications qui ciblent les versions ultérieures de EWS ne fonctionneront pas si les mêmes la fonctionnalité a été incluse dans une version antérieure. Cet article vous aideront à comprendre le rôle du schéma EWS, le fonctionnement de la gestion des versions de schéma, la relation entre la version du schéma et la version du service et la conception de votre application pour fonctionner avec le schéma EWS. 
  
## <a name="role-of-the-ews-schema"></a>Rôle du schéma EWS

Le schéma EWS effectue les opérations suivantes :
  
- Définit le jeu de fonctionnalités qui est disponible pour un client. Un client peut obtenir la liste des versions prises en charge de schéma à l’aide du [service de découverte automatique](autodiscover-for-exchange.md)de SOAP. Le client peut alors déterminer les fonctionnalités accessibles, étant donné que chaque version de schéma représente un [ensemble de fonctionnalités EWS](ews-schema-versions-in-exchange.md#bk_features). Chaque nouveau schéma publié pour EWS contient des entités de schéma à partir de la version précédente ainsi que les définitions de schéma pour les nouvelles fonctionnalités. De cette manière, EWS prend en charge les applications qui ciblent une version antérieure de EWS.
    
- Fournit une description générale du marché API. Vous pouvez utiliser ce contrat pour déterminer les structures de données pouvant être envoyés à et reçus à partir d’Exchange.
    
- Fournit un mécanisme de contrôle de version pour l’envoi de demandes. Le serveur Exchange contient toutes les versions prises en charge EWS schéma dans le répertoire virtuel. 
    
## <a name="designing-your-application-with-schema-version-in-mind"></a>Conception de votre application avec la version de schéma à l’esprit

Gardez les points suivants à l’esprit lorsque vous concevez votre application pour fonctionner avec différentes versions du schéma EWS :
  
- Activer/désactiver la fonctionnalité en fonction de la version du schéma. Vous souhaiterez mapper les fonctionnalités du client pour la version du schéma et, dans certains cas, la version du service. L’exemple suivant renverra qu'une [PropertySet](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) en fonction de la version du schéma et du service. 
    
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

- Version vos requêtes avec la version la plus ancienne du schéma EWS qui prend en charge les fonctionnalités que vous souhaitez utiliser. Cela permettra votre client applicable à un plus grand nombre de serveurs Exchange potentiels. Il est moins importante si vous développez une application métier de cibler uniquement les serveurs de votre organisation, mais il est très important si vous créez une application pour une audience plus large de Exchange.
    
## <a name="features-by-schema-version"></a>Fonctionnalités par version de schéma
<a name="bk_features"> </a>

Les versions de schéma qui sont disponibles pour un client sont identifiées dans le type simple **ExchangeVersionType** situé dans le schéma types.xsd. **ExchangeVersionType** est implémentée par l’élément [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) . L’élément **RequestServerVersion** est envoyé dans toutes les demandes EWS pour indiquer au serveur de la version du schéma les cibles de client. À son tour identifie le jeu de fonctionnalités qui est disponible pour le client. 
  
**Tableau 1 : Les fonctionnalités EWS par version de produit et de schéma**

|**Version du produit**|**Version de schéma associé**|**Fonctionnalités**|
|:-----|:-----|:-----|
|Exchange Online  |La dernière version de schéma.  |Inclut toutes les fonctionnalités dans la version actuelle d’Exchange, en plus de ces nouvelles fonctionnalités sont ajoutées pour les clients en ligne. |
|Exchange 2013 SP1 |Exchange2013_SP1 | Inclut toutes les fonctionnalités d’Exchange 2013.<br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2013 SP1 : <ul><li>[Stratégie de blocage de boîtes aux lettres](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) </li><li> [Proposer un nouvel horaire](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) </li><li>  Lire les mises à jour de l’accusé de réception pour la [mise à jour](http://msdn.microsoft.com/EN-US/library/office/dn600559%28v=exchg.80%29.aspx) et [suppression](http://msdn.microsoft.com/EN-US/library/office/dn600557%28v=exchg.80%29.aspx) d’éléments  </li><li> Mise à jour des [informations d’IRM](http://msdn.microsoft.com/EN-US/library/office/microsoft.exchange.webservices.data.conversation.hasirm%28v=exchg.80%29.aspx) pour des conversations  </li></ul> |
|Exchange 2013   |Exchange2013   | Inclut toutes les fonctionnalités introduites dans Exchange 2007 et Exchange 2010. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2013 :<ul><li>L’archivage  </li><li>  eDiscovery  </li><li>  Personnage  </li><li>  Stratégies de rétention  </li><li>  Magasin de contacts unifié  </li><li>  Photos de l’utilisateur  </li></ul> |
|Exchange 2010 SP2   |Exchange2010_SP2 | Inclut toutes les fonctionnalités introduites dans Exchange 2010 SP1. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP2 :<ul><li>Obtenir l’Expiration du mot de passe  </li><li>  Précision DateTime  </li><li>  Identificateurs de propriété mis à jour pour les contacts  </li><li>  Nouveaux scénarios de l’emprunt d’identité  </li></ul> |
|Exchange 2010 SP1  |Exchange2010_SP1   | Inclut toutes les fonctionnalités introduites dans Exchange 2010. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2010 SP1 :<ul><li>Créer, récupérer et modifier des règles de boîte de réception  </li><li>  Accès par programme aux boîtes aux lettres d’Archive  </li><li>  Actions de conversations  </li><li>  Le parcours des notifications de pare-feu  </li><li>  Fonctionnalités d’administration améliorée  </li><li>  Amélioration de la prise en charge de la version mixte  </li><li>  Limitation de la prise en charge de la protection  </li><li>  Contrôle d’accès application EWS  </li><li>  Prise en charge de l’authentification de certificat client  </li></ul> |
|Exchange 2010  |Exchange2010   | Inclut toutes les fonctionnalités introduites dans Exchange 2007 SP1. <br/><br/>Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2010 :<ul><li>Liste de Distribution privée complète  </li><li>  Objets de Configuration utilisateur  </li><li>  Dossier des éléments associés  </li><li>  Suivi des messages  </li><li>  Messagerie unifiée  </li><li>  Découverte automatique SOAP  </li><li>  Prise en charge améliorée de fuseau horaire  </li><li>  Informations de disponibilité de ressources de salle  </li><li>  Recherche indexés  </li><li>  Accès benne  </li><li>  Partage des informations  </li></ul> |
|Exchange 2007 SP1   |Exchange2007_SP1  | Inclut toutes les fonctionnalités introduites dans Exchange 2007. <br/><br/>Les fonctionnalités suivantes ont été introduites dans Exchange 2007 SP1 :<ul><li>Gestion des délégués  </li><li>  Autorisations de dossier  </li><li>  Dossiers publics  </li><li>  Publier des éléments  </li><li>  Conversion de l’ID  </li></ul>|
|Exchange 2007  |Exchange2007 | Les fonctionnalités suivantes ont été introduites dans la version initiale d’Exchange 2007 :<ul><li>Accès total aux éléments, dossiers et pièces jointes (créer, obtenir, mettre à jour, supprimer)  </li><li>  Disponibilité  </li><li>  En dehors des paramètres Office  </li><li>  Notifications  </li><li>  Synchronisation  </li><li>  Résolution de noms  </li><li>  Extension de la distribution (liste)  </li><li>  Search  </li></ul> |
   
## <a name="relationship-between-the-ews-schema-and-the-service-version"></a>Relation entre le schéma EWS et la version du service
<a name="bk_features"> </a>

La version du schéma EWS est liée à la version du service EWS que le serveur est en cours d’exécution. Le modèle d’affectation de noms pour le schéma EWS est lié aux versions d’Exchange sur site. Par exemple, la version initiale d’Exchange 2013 a une version de service de 15.00.0516.032 et le nom de schéma **Exchange2013**. Étant donné que le schéma a été mis à jour pour Exchange 2013, Exchange 2013 et Exchange Online avec une version de service de 15.00.0516.032 et versions ultérieures ont le même nom de version du schéma le plus récent. Dans les versions antérieures d’Exchange, le schéma EWS n’a été pas mis à jour avec les mises à jour cumulatives (anciennement appelé cumulatifs). Mais Exchange est plus souvent mis à jour pour prendre en charge Exchange Online, mises à jour cumulatives contiennent désormais des mises à jour de schéma pour EWS. Les noms de fichier de schéma et le nom de version de schéma associé, sont uniquement mis à jour avec les service packs ou les versions majeures de Exchange sur site.
  
Pendant que le schéma EWS définit le contrat, dans certains scénarios, la version du service est le seul moyen pour un client déterminer la façon dont il est supposé pour interagir avec le service. Changements de comportement de service qui ne figurent pas dans le schéma ne peuvent pas être déterminées par la version de service renvoyée dans toutes les réponses EWS. Par exemple, lorsque [les dossiers publics](public-folder-access-with-ews-in-exchange.md) ont été repensées dans Exchange 2013, les opérations qui permettent de déplacer et copier des dossiers publics est modifiées. Si vous avez créé un client pour copier les dossiers publics dans Exchange 2010, vous devez mettre à jour pour les différentes opérations permet d’obtenir le même résultat dans Exchange 2013. 
  
## <a name="how-the-ews-schema-is-updated"></a>Comment le schéma EWS est mis à jour
<a name="bk_features"> </a>

Les serveurs exécutant des versions d’Exchange commençant par Exchange 2007 incluent le schéma EWS dans le répertoire virtuel qui héberge le service EWS. La version du schéma actuel est toujours représentée par les fichiers types.xsd et messages.xsd. La figure 1 illustre la façon dont le schéma messages.xsd est redirigé lorsqu’une nouvelle version du schéma est développée. Avant d’ajouter de nouvelles fonctionnalités, une copie du schéma messages.xsd d’origine est incluse et renommée pour représenter la version précédente du schéma. Le fichier messages.xsd est alors mis à jour avec la description de service pour la nouvelle version.
  
**La figure 1. Comment le schéma EWS est mis à jour**

![Illustration de la mise à jour du schéma EWS. La dernière version du schéma est divisée et renommée afin de représenter la version précédente et le dernier nom de fichier représente la version actuelle.](media/Ex15_EWS_Schema_Update1.png)
  
Avant le schéma EWS est mis à jour d’une nouvelle version, la version actuelle du schéma est redirigée et renommées à l’aide de la convention suivante :
  
`<schemaname>-<majorserverversion><servicepack>.xsd`
  
Le nom du fichier d’origine puis représente le schéma le plus récent. Toutes les nouvelles fonctionnalités sont ajoutées au schéma le plus récent, à l’exception des mises à jour et des correctifs pour les versions antérieures du schéma. 
  
## <a name="see-also"></a>Voir aussi

- [Versions de schéma EWS dans Exchange](ews-schema-versions-in-exchange.md) 
- [Découverte automatique pour Exchange](autodiscover-for-exchange.md) 
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

