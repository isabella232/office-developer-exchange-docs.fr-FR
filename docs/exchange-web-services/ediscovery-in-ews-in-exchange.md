---
title: découverte électronique dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Découvrez la fonctionnalité eDiscovery dans EWS dans Exchange.
ms.openlocfilehash: 48e3fdb3a2f21f7dcfcb7eed21b586e099b249a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456093"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="97e5e-103">découverte électronique dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97e5e-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="97e5e-104">Découvrez la fonctionnalité eDiscovery dans EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="97e5e-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="97e5e-105">eDiscovery est un service Web de requête fédérée qui permet aux applications externes d’exécuter des requêtes de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="97e5e-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="97e5e-106">La découverte se compose de plusieurs phases, y compris l’identification et la conservation des données clés, le Culling et l’examen des données, ainsi que la production de données en justice.</span><span class="sxs-lookup"><span data-stu-id="97e5e-106">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court.</span></span> <span data-ttu-id="97e5e-107">les requêtes eDiscovery facilitent le processus de découverte en fournissant un flux de travail de découverte unique entre Exchange et SharePoint.</span><span class="sxs-lookup"><span data-stu-id="97e5e-107">eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="97e5e-108">opérations eDiscovery</span><span class="sxs-lookup"><span data-stu-id="97e5e-108">eDiscovery operations</span></span>

<span data-ttu-id="97e5e-109">La fonctionnalité de découverte électronique exposée par EWS est disponible via les opérations introduites dans Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange à partir d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="97e5e-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with Exchange 2013.</span></span> 
  
<span data-ttu-id="97e5e-110">**Tableau 1. Nouvelles opérations pour eDiscovery**</span><span class="sxs-lookup"><span data-stu-id="97e5e-110">**Table 1. New operations for eDiscovery**</span></span>

|<span data-ttu-id="97e5e-111">**Nom de l’opération**</span><span class="sxs-lookup"><span data-stu-id="97e5e-111">**Operation name**</span></span>|<span data-ttu-id="97e5e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="97e5e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97e5e-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="97e5e-113">GetDiscoverySearchConfiguration</span></span>](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-114">Obtient les informations de configuration pour les conservations inaltérables, les recherches de découverte enregistrées et les boîtes aux lettres qui sont activées pour la recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="97e5e-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="97e5e-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e5e-115">GetHoldOnMailboxes</span></span>](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-116">Obtient l’état d’une conservation basée sur une requête, qui est définie à l’aide de l' [opération SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="97e5e-116">Gets the status of a query-based hold, which is set by using the [SetHoldOnMailboxes operation](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="97e5e-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="97e5e-117">GetNonIndexableItemDetails</span></span>](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-118">Récupère des détails sur les éléments qui ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="97e5e-118">Retrieves details about items that cannot be indexed.</span></span> <span data-ttu-id="97e5e-119">Cela inclut, sans s’y limiter, l’identificateur de l’élément, un code d’erreur, une description de l’erreur, lorsqu’une tentative d’indexation de l’élément est effectuée, ainsi que des informations supplémentaires sur le fichier.</span><span class="sxs-lookup"><span data-stu-id="97e5e-119">This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="97e5e-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="97e5e-120">GetNonIndexableItemStatistics</span></span>](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-121">Récupère le nombre d’éléments qui ne peuvent pas être indexés dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="97e5e-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="97e5e-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e5e-122">GetSearchableMailboxes</span></span>](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-123">Obtient la liste des boîtes aux lettres pour lesquelles le client est autorisé à effectuer des recherches ou à exécuter la fonctionnalité eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="97e5e-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="97e5e-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e5e-124">SearchMailboxes</span></span>](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-125">Recherche des éléments dans des boîtes aux lettres spécifiques qui correspondent à des mots clés de requête.</span><span class="sxs-lookup"><span data-stu-id="97e5e-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="97e5e-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="97e5e-126">SetHoldOnMailboxes</span></span>](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="97e5e-127">Définit une conservation basée sur une requête sur des éléments.</span><span class="sxs-lookup"><span data-stu-id="97e5e-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97e5e-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97e5e-128">See also</span></span>

- [<span data-ttu-id="97e5e-129">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="97e5e-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="97e5e-130">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97e5e-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="97e5e-131">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="97e5e-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

