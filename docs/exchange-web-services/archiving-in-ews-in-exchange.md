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
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="d9eb3-103">L’archivage dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d9eb3-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="d9eb3-104">Obtenir des informations sur l’archivage dans EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="d9eb3-105">Boîtes aux lettres d’archivage sont des boîtes aux lettres secondaires qui sont associés à un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-105">Archive mailboxes are secondary mailboxes that are associated with a user.</span></span> <span data-ttu-id="d9eb3-106">Boîtes aux lettres d’archivage sont généralement utilisés pour gérer les limites de stockage de courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-106">Archive mailboxes are typically used to manage email storage limits.</span></span> <span data-ttu-id="d9eb3-107">Par exemple, les éléments de messagerie électronique antérieurs régulièrement peuvent être déplacés que de la boîte de réception à la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-107">For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="d9eb3-108">Exchange Online, Exchange Online dans le cadre d’Office 365 et Exchange Server 2013 présente deux nouvelles opérations Exchange Web Services (EWS) que vous pouvez utiliser pour archiver un ensemble d’éléments de messagerie à partir d’une boîte aux lettres principale.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="d9eb3-109">L’archivage des éléments de boîte de réception de cette manière conserve la hiérarchie de dossiers des éléments.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="d9eb3-110">En outre, les boîtes aux lettres d’archive maintenant peuvent être stockées localement sur un client, soit à distance, d’une manière qui est principalement opaque à un utilisateur, à l’aide d’un chemin d’accès du dossier pour pointer vers le contenu de l’archive.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="d9eb3-111">Opérations d’archivage dans EWS</span><span class="sxs-lookup"><span data-stu-id="d9eb3-111">Archiving operations in EWS</span></span>

<span data-ttu-id="d9eb3-112">Le tableau suivant répertorie les opérations d’archivage qui ont été introduites dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="d9eb3-113">**Nom de l’opération**</span><span class="sxs-lookup"><span data-stu-id="d9eb3-113">**Operation name**</span></span>|<span data-ttu-id="d9eb3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d9eb3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9eb3-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="d9eb3-115">ArchiveItem</span></span>](http://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="d9eb3-116">Déplace un élément à partir de la boîte aux lettres principale pour la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d9eb3-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="d9eb3-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="d9eb3-118">Crée un URI qui pointe vers l’emplacement de stockage pour la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="d9eb3-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9eb3-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d9eb3-119">See also</span></span>

- [<span data-ttu-id="d9eb3-120">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d9eb3-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="d9eb3-121">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d9eb3-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="d9eb3-122">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d9eb3-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

