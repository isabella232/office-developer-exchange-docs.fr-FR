---
title: L'archivage dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Découvrez l’archivage dans EWS dans Exchange.
ms.openlocfilehash: f2ca4cc783556b089b732c75d166b77c0dcd891c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520226"
---
# <a name="archiving-in-ews-in-exchange"></a>L'archivage dans EWS dans Exchange

Découvrez l’archivage dans EWS dans Exchange.
  
Les boîtes aux lettres d’archivage sont des boîtes aux lettres secondaires associées à un utilisateur. Les boîtes aux lettres d’archivage sont généralement utilisées pour gérer les limites de stockage de messagerie. Par exemple, des éléments de courrier plus anciens peuvent régulièrement être déplacés de la boîte de réception vers la boîte aux lettres d’archivage. 
  
Exchange Online, Exchange Online dans le cadre de Office 365 et Exchange Server 2013 introduisent deux nouvelles opérations des services web Exchange (EWS) que vous pouvez utiliser pour archiver un ensemble d’éléments de messagerie à partir d’une boîte aux lettres principale. L’archivage des éléments de la boîte de réception de cette façon conserve la hiérarchie de dossiers des éléments. En outre, les boîtes aux lettres d’archivage peuvent désormais être stockées localement sur un client ou à distance, d’une manière qui est principalement opaque pour un utilisateur, à l’aide d’un chemin d’accès de dossier pour pointer vers le contenu de l’archive.
  
## <a name="archiving-operations-in-ews"></a>Opérations d’archivage dans EWS

Le tableau suivant répertorie les opérations d’archivage qui ont été introduites Exchange 2013. 
  
|**Nom de l’opération**|**Description**|
|:-----|:-----|
|[ArchiveItem](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |Déplace un élément de la boîte aux lettres principale vers la boîte aux lettres d’archivage.  <br/> |
|[CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |Crée un URI qui pointe vers l’emplacement de stockage de la boîte aux lettres d’archivage.  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

