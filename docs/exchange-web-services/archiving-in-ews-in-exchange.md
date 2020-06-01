---
title: L'archivage dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Découvrez l’archivage dans EWS dans Exchange.
ms.openlocfilehash: b433b9f88905ee255720e8b341d560fa0e464975
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456212"
---
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="ba7a2-103">L'archivage dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba7a2-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="ba7a2-104">Découvrez l’archivage dans EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="ba7a2-105">Les boîtes aux lettres d’archivage sont des boîtes aux lettres secondaires associées à un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-105">Archive mailboxes are secondary mailboxes that are associated with a user.</span></span> <span data-ttu-id="ba7a2-106">Les boîtes aux lettres d’archivage sont généralement utilisées pour gérer les limites de stockage des courriers électroniques.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-106">Archive mailboxes are typically used to manage email storage limits.</span></span> <span data-ttu-id="ba7a2-107">Par exemple, les éléments de courrier plus anciens peuvent régulièrement être déplacés de la boîte de réception vers la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-107">For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="ba7a2-108">Exchange Online, Exchange Online dans le cadre d’Office 365 et Exchange Server 2013 introduisent deux nouvelles opérations des services Web Exchange (EWS) que vous pouvez utiliser pour archiver un ensemble d’éléments de courrier à partir d’une boîte aux lettres principale.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="ba7a2-109">L’archivage des éléments de boîte de réception de cette manière conserve la hiérarchie des dossiers des éléments.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="ba7a2-110">En outre, les boîtes aux lettres d’archivage peuvent désormais être stockées localement sur un client, ou à distance, d’une manière qui est principalement opaque pour un utilisateur, en utilisant un chemin d’accès de dossier pour pointer vers le contenu de l’archive.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="ba7a2-111">Opérations d’archivage dans EWS</span><span class="sxs-lookup"><span data-stu-id="ba7a2-111">Archiving operations in EWS</span></span>

<span data-ttu-id="ba7a2-112">Le tableau suivant répertorie les opérations d’archivage qui ont été introduites dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="ba7a2-113">**Nom de l’opération**</span><span class="sxs-lookup"><span data-stu-id="ba7a2-113">**Operation name**</span></span>|<span data-ttu-id="ba7a2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba7a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba7a2-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="ba7a2-115">ArchiveItem</span></span>](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="ba7a2-116">Déplace un élément de la boîte aux lettres principale vers la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ba7a2-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="ba7a2-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="ba7a2-118">Crée un URI qui pointe vers l’emplacement de stockage de la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="ba7a2-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba7a2-119">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba7a2-119">See also</span></span>

- [<span data-ttu-id="ba7a2-120">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ba7a2-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="ba7a2-121">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba7a2-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="ba7a2-122">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ba7a2-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

