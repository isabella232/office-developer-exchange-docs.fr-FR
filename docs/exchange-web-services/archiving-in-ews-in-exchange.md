---
title: L’archivage dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Obtenir des informations sur l’archivage dans EWS dans Exchange.
ms.openlocfilehash: bc282a7774bb74e57550bc663512987839324b83
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754755"
---
# <a name="archiving-in-ews-in-exchange"></a>L’archivage dans EWS dans Exchange

Obtenir des informations sur l’archivage dans EWS dans Exchange.
  
Boîtes aux lettres d’archivage sont des boîtes aux lettres secondaires qui sont associés à un utilisateur. Boîtes aux lettres d’archivage sont généralement utilisés pour gérer les limites de stockage de courrier électronique. Par exemple, les éléments de messagerie électronique antérieurs régulièrement peuvent être déplacés que de la boîte de réception à la boîte aux lettres d’archive. 
  
Exchange Online, Exchange Online dans le cadre d’Office 365 et Exchange Server 2013 présente deux nouvelles opérations Exchange Web Services (EWS) que vous pouvez utiliser pour archiver un ensemble d’éléments de messagerie à partir d’une boîte aux lettres principale. L’archivage des éléments de boîte de réception de cette manière conserve la hiérarchie de dossiers des éléments. En outre, les boîtes aux lettres d’archive maintenant peuvent être stockées localement sur un client, soit à distance, d’une manière qui est principalement opaque à un utilisateur, à l’aide d’un chemin d’accès du dossier pour pointer vers le contenu de l’archive.
  
## <a name="archiving-operations-in-ews"></a>Opérations d’archivage dans EWS

Le tableau suivant répertorie les opérations d’archivage qui ont été introduites dans Exchange 2013. 
  
|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[ArchiveItem](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Déplace un élément à partir de la boîte aux lettres principale pour la boîte aux lettres d’archive.  <br/> |
|[CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Crée un URI qui pointe vers l’emplacement de stockage pour la boîte aux lettres d’archive.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

