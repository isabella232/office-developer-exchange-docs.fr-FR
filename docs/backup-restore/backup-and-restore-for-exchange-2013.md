---
title: Sauvegarde et restauration pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Trouvez des informations sur la création de sauvegarde et de restauration des applications pour Exchange 2013.
ms.openlocfilehash: 9eceb3d512a73ad9cb07a01864fb8b029d5b5772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754743"
---
# <a name="backup-and-restore-for-exchange"></a>Sauvegarde et restauration pour Exchange
  
Exchange Server 2013 fournit des groupes de disponibilité de base de données (DAG), qui permet de conserver les données stockées sécurisées et disponibles et réduisent la nécessité de sauvegarde personnalisée et restaurer des applications. DAG activer la redondance des données hors site pour vous assurer que vous ne perdre des données. Toutefois, plusieurs plans de récupération d’urgence continuent inclure plus conventionnelle sauvegarde et la restauration des méthodes et des systèmes, y compris des applications personnalisées pour la redondance avec le DAG. Pour garantir la disponibilité des données et à la redondance dans votre organisation, vous pouvez créer des applications personnalisées qui utilisent les technologies de système d’exploitation Exchange Server et Windows Server pour sauvegarder et restaurer vos données Exchange.

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Technologies de sauvegarde d’Exchange 2013

Exchange 2013 comprend un plug-in pour la sauvegarde de Windows Server qui permet aux administrateurs d’effectuer des sauvegardes VSS des données Exchange. Les administrateurs peuvent également utiliser sauvegarde Windows Server pour sauvegarder et restaurer des bases de données Exchange. Si vous créez une sauvegarde et restaurez d’application pour Exchange 2013, vous devez créer une application compatible avec Exchange qui prend en charge de l’enregistreur VSS pour Exchange 2013 et utiliser l’API CHKSGFILES pour valider la cohérence de la sauvegarde. Pour plus d’informations, voir [l’intégrité des sauvegardes de valider en utilisant l’API CHKSGFILES dans Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Enregistreur VSS dans Exchange 2013

Exchange 2013 présente des modifications importantes à l’architecture d’enregistreur VSS dans Exchange Server 2010 et Exchange Server 2007. Exchange 2010 et Exchange 2007 sont deux enregistreurs VSS : un à l’intérieur du service banque d’informations Exchange (store.exe) et l’autre à l’intérieur du service de réplication Exchange (msexchangerepl.exe). Dans Exchange 2013, la fonctionnalité d’enregistreur VSS se trouve dans le service de réplication Exchange. Votre application de sauvegarde et de restauration utilise le nouveau rédacteur VSS, appelé l’auteur du message Microsoft Exchange, pour sauvegarder des copies de base de données actives et passives et pour restaurer une sauvegarde de copies de base de données. Le rédacteur VSS nouvel s’exécute dans le service de réplication Exchange, le service banque d’informations Exchange doit être exécuté dans l’ordre de l’enregistreur soit disponible. Par conséquent, les deux services sont nécessaires pour sauvegarder ou restaurer des bases de données Exchange.
  
Bien que l’architecture du rédacteur VSS a été mis à jour dans Exchange 2013, la fonctionnalité sous-jacente n’a pas changé. Si vous avez créé une application de sauvegarde et de restauration pour Exchange 2010, il est inutile d’apporter des modifications à votre application pour Exchange 2013. Veillez à recompiler votre application avec les derniers fichiers pour assurer la compatibilité. Pour les applications de sauvegarde et de restauration créées pour Exchange 2007 ou versions antérieures, vous devrez réécrire votre code pour utiliser l’API CHKSGFILES le plus récent.
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>Ce que vous devez savoir à propos de restauration et sauvegarde VSS

|Si vous vous interrogez sur...|Voici la réponse|
|:-----|:-----|
|Architectures d'application  <br/> |Sauvegarde et restauration des applications qui utilisent VSS pour sauvegarder les bases de données généralement consistant d’un service d’arrière-plan qui effectue la sauvegarde, un service de planification et une console d’application GUI Windows qui contrôle et configure la sauvegarde et restauration du système Exchange.  <br/> |
|Utilisation à distance  <br/> |Les applications qui utilisent le service VSS pour sauvegarder des serveurs Exchange doivent s’exécuter sur l’ordinateur Windows Server 2008 sur lequel est exécuté le processus de banque Exchange. En raison de la flexibilité dans des systèmes de stockage de grande taille, le matériel hébergeant les volumes de stockage physique peut-être pas partie de l’ordinateur qui exécute Windows Server 2008.  <br/> |
|Langages et outils  <br/> |Vous pouvez utiliser n’importe quel langage compatible COM pour utiliser VSS. Il est fréquemment utilisé dans les applications écrites en langage C++. Étant donné que vous devez suivre la banque d’informations Exchange en mode hors connexion pour créer des clichés instantanés, les applications de sauvegarde sont généralement sensible au temps, qui dans la plupart des cas, facilite l’utilisation des langages tels que Visual Basic ou VBScript pas pratique.  <br/> |
|Implémentation managée  <br/> |Vous pouvez utiliser les API VSS dans un environnement de code managé par le biais d’un Assembly d’interopérabilité COM.  <br/> |
|Peut contenir des scripts  <br/> |Oui, mais pas recommandé.  <br/> |
|Les outils de test et de débogage disponibles  <br/> |Aucun des outils spéciaux ne sont requis pour déboguer des applications qui utilisent le VSS de Windows.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section

- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Créer la sauvegarde et de restaurer des applications pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>Voir aussi

- [Volume Shadow Copy Service (Windows)](http://msdn.microsoft.com/en-us/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Explorer l'API managée EWS, EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Agents de transport dans Exchange](../transport-agents/transport-agents-in-exchange-2013.md) 
    

