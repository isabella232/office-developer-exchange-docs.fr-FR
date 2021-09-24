---
title: Sauvegarde et restauration pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Trouvez des informations sur la création d’applications de sauvegarde et de restauration Exchange 2013.
ms.openlocfilehash: 2be8295985651319860ab2d2a143d69f663bf932
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514899"
---
# <a name="backup-and-restore-for-exchange"></a>Sauvegarde et restauration pour Exchange
  
Exchange Server 2013 fournit des groupes de disponibilité de base de données (DG), qui permettent de garantir la sécurité et la disponibilité des données stockées, et de réduire le besoin d’applications de sauvegarde et de restauration personnalisées. Les DG activent la redondance des données hors site pour vous assurer que vous ne perdrez pas de données. Toutefois, de nombreux plans de récupération d’urgence continuent d’inclure des méthodes et des systèmes de sauvegarde et de restauration plus traditionnels, y compris des applications personnalisées, pour la redondance avec le DAG. Pour garantir la disponibilité et la redondance des données dans votre organisation, vous pouvez créer des applications personnalisées qui utilisent les technologies du système d’exploitation Exchange Server et Windows Server pour la protection et la restauration de vos données Exchange données.

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Technologies de sauvegarde Exchange 2013

Exchange 2013 inclut un plug-in pour la sauvegarde Windows Server que les administrateurs peuvent utiliser pour effectuer des sauvegardes VSS de Exchange données. Les administrateurs peuvent également utiliser Windows sauvegarde de serveur pour sauvegarder et restaurer Exchange bases de données. Si vous créez une application de sauvegarde et de restauration pour Exchange 2013, vous devez créer une application Exchange qui prend en charge le rédacteur VSS pour Exchange 2013 et utiliser l’API CHKSGFILES pour valider la cohérence de cette sauvegarde. Pour plus d’informations, voir Valider l’intégrité de la sauvegarde à l’aide de [l’API CHKSGFILES Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Rédacteur VSS dans Exchange 2013

Exchange 2013 introduit une modification significative de l’architecture du rédacteur VSS dans Exchange Server 2010 et Exchange Server 2007. Exchange 2010 et Exchange 2007 incluent deux rédacteurs VSS : un à l’intérieur du service de magasin d’informations Exchange (store.exe) et un autre à l’intérieur du service de réplication Exchange (msexchangerepl.exe). Dans Exchange 2013, la fonctionnalité d’écriture VSS se trouve dans le service Exchange réplication. Votre application de sauvegarde et de restauration utilise le nouvel rédacteur VSS, appelé Rédacteur Microsoft Exchange, pour sauvegarder les copies de base de données actives et passives, et pour restaurer les copies de base de données restaurées. Bien que le nouvel rédacteur VSS s’exécute dans le service de réplication Exchange, le service de magasin d’informations Exchange doit être en cours d’exécution pour que le rédacteur soit disponible. Par conséquent, les deux services sont nécessaires pour sauvegarder ou restaurer des bases de données Exchange.
  
Bien que l’architecture du rédacteur VSS ait été mise à jour Exchange 2013, la fonctionnalité sous-jacente n’a pas changé. Si vous avez créé une application de sauvegarde et de restauration pour Exchange 2010, vous n’avez pas besoin d’apporter des modifications à votre application pour Exchange 2013. Veillez à recompiler votre application avec les derniers fichiers pour garantir la compatibilité. Pour les applications de sauvegarde et de restauration créées pour Exchange 2007 ou versions antérieures, vous devez réécrire votre code pour utiliser la dernière API CHKSGFILES.
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>Ce que vous devez savoir sur la sauvegarde et la restauration VSS

|Si vous vous demandez à propos de...|Voici la réponse|
|:-----|:-----|
|Architectures d'application  <br/> |Les applications de sauvegarde et de restauration qui utilisent VSS pour sauvegarder des bases de données Exchange se composent généralement d’un service d’arrière-plan qui effectue la sauvegarde, d’un service de planification et d’une console d’application GRAPHIQUE Windows qui contrôle et configure le système de sauvegarde et de restauration.  <br/> |
|Utilisation à distance  <br/> |Les applications qui utilisent VSS pour la Exchange serveurs doivent s’exécuter sur l’ordinateur Windows Server 2008 sur lequel le processus Exchange store est en cours d’exécution. En raison de la flexibilité des systèmes de stockage de grande taille, le matériel hébergeant les volumes de stockage peut ne pas faire partie physiquement de l’ordinateur exécutant Windows Server 2008.  <br/> |
|Langages et outils  <br/> |Vous pouvez utiliser n’importe quel langage compatible COM pour utiliser VSS. Il est le plus souvent utilisé dans les applications écrites en C++. Étant donné que vous devez mettre le magasin Exchange hors connexion pour créer des copies de secours, les applications de sauvegarde sont généralement sensibles au temps, ce qui rend dans la plupart des cas l’utilisation de langages comme Visual Basic ou VBScript non pratique.  <br/> |
|Implémentation managée  <br/> |Vous pouvez utiliser les API VSS dans un environnement de code géré via un assembly COM Interop.  <br/> |
|Peut contenir des scripts  <br/> |Oui, mais non recommandé.  <br/> |
|Les outils de test et de débogage disponibles  <br/> |Aucun outil spécial n’est requis pour déboguer les applications qui utilisent Windows VSS.  <br/> |
   
## <a name="in-this-section"></a>Dans cette section

- [Concepts de sauvegarde et de restauration pour Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Créer des applications de sauvegarde et de restauration pour Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Référence de classe CChkSGFiles](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>Voir aussi

- [Service de copie de l’ombre de volume (Windows)](https://msdn.microsoft.com/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Explorer l'API managée EWS, l’EWS et les services web dans Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Agents de transport dans Exchange](../transport-agents/transport-agents-in-exchange-2013.md) 
    

