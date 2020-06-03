---
title: Sauvegarde et restauration pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Trouvez des informations sur la création d’applications de sauvegarde et de restauration pour Exchange 2013.
ms.openlocfilehash: 1c5d99be60501fd1c4414ea22294bd05645bb0a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455239"
---
# <a name="backup-and-restore-for-exchange"></a>Sauvegarde et restauration pour Exchange
  
Exchange Server 2013 fournit des groupes de disponibilité de base de données (DAG), qui permettent de maintenir la sécurité et la disponibilité des données stockées, tout en réduisant la nécessité d’utiliser des applications de sauvegarde et de restauration personnalisées. Dag active la redondance des données hors site pour vous assurer que vous ne perdez pas de données. Toutefois, de nombreux plans de récupération d’urgence continuent d’inclure des méthodes et des systèmes de sauvegarde et de restauration plus traditionnels, y compris des applications personnalisées, pour la redondance avec le DAG. Pour garantir la disponibilité et la redondance des données au sein de votre organisation, vous pouvez créer des applications personnalisées qui utilisent les technologies de système d’exploitation Exchange Server et Windows Server pour sauvegarder et restaurer vos données Exchange.

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Technologies de sauvegarde dans Exchange 2013

Exchange 2013 inclut un plug-in pour la sauvegarde Windows Server que les administrateurs peuvent utiliser pour effectuer des sauvegardes VSS des données Exchange. Les administrateurs peuvent également utiliser la sauvegarde Windows Server pour sauvegarder et restaurer des bases de données Exchange. Si vous créez une application de sauvegarde et de restauration pour Exchange 2013, vous devez créer une application compatible Exchange qui prend en charge l’enregistreur VSS pour Exchange 2013 et utiliser l’API CHKSGFILES pour valider la cohérence de cette sauvegarde. Pour plus d’informations, consultez la rubrique validation de l' [intégrité de la sauvegarde à l’aide de l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Enregistreur VSS dans Exchange 2013

Exchange 2013 introduit une modification significative de l’architecture de l’enregistreur VSS dans Exchange Server 2010 et Exchange Server 2007. Exchange 2010 et Exchange 2007 incluent deux enregistreurs VSS : un à l’intérieur du service de banque d’informations Exchange (Store. exe) et un dans le service de réplication Exchange (MSExchangeRepl. exe). Dans Exchange 2013, la fonctionnalité d’enregistreur VSS se trouve dans le service de réplication Exchange. Votre application de sauvegarde et de restauration utilise le nouvel enregistreur VSS, appelé le rédacteur Microsoft Exchange, pour sauvegarder les copies de base de données actives et passives et restaurer les copies de base de données sauvegardées. Bien que le nouvel enregistreur VSS s’exécute dans le service de réplication Exchange, le service de banque d’informations Exchange doit être en cours d’exécution pour que le writer soit disponible. Par conséquent, les deux services sont nécessaires pour sauvegarder ou restaurer des bases de données Exchange.
  
Bien que l’architecture de l’enregistreur VSS ait été mise à jour dans Exchange 2013, la fonctionnalité sous-jacente n’a pas changé. Si vous avez créé une application de sauvegarde et de restauration pour Exchange 2010, vous n’avez pas besoin d’effectuer des modifications dans votre application pour Exchange 2013. Assurez-vous de recompiler votre application avec les fichiers les plus récents pour garantir la compatibilité. Pour les applications de sauvegarde et de restauration créées pour Exchange 2007 ou des versions antérieures, vous devrez réécrire votre code pour utiliser la dernière API CHKSGFILES.
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>Ce que vous devez savoir sur la sauvegarde et la restauration de VSS

|Si vous vous posez des informations sur...|Voici la réponse|
|:-----|:-----|
|Architectures d'application  <br/> |Les applications de sauvegarde et de restauration qui utilisent VSS pour sauvegarder des bases de données Exchange se composent généralement d’un service d’arrière-plan qui effectue la sauvegarde, un service de planification et une console d’application Windows GUI qui contrôle et configure le système de sauvegarde et de restauration.  <br/> |
|Utilisation à distance  <br/> |Les applications qui utilisent VSS pour sauvegarder des serveurs Exchange doivent s’exécuter sur l’ordinateur Windows Server 2008 sur lequel le processus de la Banque d’Exchange est en cours d’exécution. En raison de la flexibilité des systèmes de stockage de grande taille, le matériel qui héberge les volumes de stockage ne doit pas nécessairement faire partie de l’ordinateur qui exécute Windows Server 2008.  <br/> |
|Langages et outils  <br/> |Vous pouvez utiliser n’importe quel langage compatible COM pour utiliser VSS. Il est le plus souvent utilisé dans les applications écrites en C++. Étant donné que vous devez déconnecter la Banque d’informations Exchange pour créer des clichés instantanés, les applications de sauvegarde sont généralement sensibles au temps, ce qui peut, dans la plupart des cas, utiliser des langages tels que Visual Basic ou VBScript.  <br/> |
|Implémentation managée  <br/> |Vous pouvez utiliser les API VSS dans un environnement de code managé via un assembly d’interopérabilité COM.  <br/> |
|Peut contenir des scripts  <br/> |Oui, mais non recommandé.  <br/> |
|Les outils de test et de débogage disponibles  <br/> |Aucun outil spécial n’est requis pour déboguer les applications qui utilisent le service VSS Windows.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section

- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Référence de classe fonction cchksgfiles](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>Voir aussi

- [Service de cliché instantané des volumes (Windows)](https://msdn.microsoft.com/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Agents de transport dans Exchange](../transport-agents/transport-agents-in-exchange-2013.md) 
    

