---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: L’élément FindMailboxStatisticsByKeywords spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé.
ms.openlocfilehash: e667f13b66e439dca88d73a5e05d74846183928c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756401"
---
# <a name="findmailboxstatisticsbykeywords"></a><span data-ttu-id="17265-103">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="17265-103">FindMailboxStatisticsByKeywords</span></span>

<span data-ttu-id="17265-104">L’élément **FindMailboxStatisticsByKeywords** spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé.</span><span class="sxs-lookup"><span data-stu-id="17265-104">The **FindMailboxStatisticsByKeywords** element specifies a request to search for mailbox statistics by keyword.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 <span data-ttu-id="17265-105">**FindMailboxStatisticsByKeywordsType**</span><span class="sxs-lookup"><span data-stu-id="17265-105">**FindMailboxStatisticsByKeywordsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17265-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="17265-106">Attributes and elements</span></span>

<span data-ttu-id="17265-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="17265-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17265-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="17265-108">Attributes</span></span>

<span data-ttu-id="17265-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="17265-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17265-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="17265-110">Child elements</span></span>

|<span data-ttu-id="17265-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="17265-111">**Element**</span></span>|<span data-ttu-id="17265-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="17265-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17265-113">Boîtes aux lettres (ArrayOfUserMailboxesType)</span><span class="sxs-lookup"><span data-stu-id="17265-113">Mailboxes (ArrayOfUserMailboxesType)</span></span>](mailboxes-arrayofusermailboxestype.md) <br/> |<span data-ttu-id="17265-114">Contient un tableau de boîtes aux lettres affectées par la suspension.</span><span class="sxs-lookup"><span data-stu-id="17265-114">Contains an array of mailboxes affected by the hold.</span></span>  <br/> |
|[<span data-ttu-id="17265-115">Mots clés</span><span class="sxs-lookup"><span data-stu-id="17265-115">Keywords</span></span>](keywords-ex15websvcsotherref.md) <br/> |<span data-ttu-id="17265-116">Spécifie les mots clés pour une recherche.</span><span class="sxs-lookup"><span data-stu-id="17265-116">Specifies keywords for a search.</span></span>  <br/> |
|[<span data-ttu-id="17265-117">Language</span><span class="sxs-lookup"><span data-stu-id="17265-117">Language</span></span>](language.md) <br/> |<span data-ttu-id="17265-118">Contient la langue utilisée pour la requête de recherche.</span><span class="sxs-lookup"><span data-stu-id="17265-118">Contains the language used for the search query.</span></span>  <br/> |
|[<span data-ttu-id="17265-119">Expéditeurs</span><span class="sxs-lookup"><span data-stu-id="17265-119">Senders</span></span>](senders.md) <br/> |<span data-ttu-id="17265-120">Spécifie un tableau d’adresses SMTP.</span><span class="sxs-lookup"><span data-stu-id="17265-120">Specifies an array of SMTP addresses.</span></span>  <br/> |
|[<span data-ttu-id="17265-121">Destinataires (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="17265-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="17265-122">Spécifie un tableau de destinataires d’un message.</span><span class="sxs-lookup"><span data-stu-id="17265-122">Specifies an array of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="17265-123">FromDate</span><span class="sxs-lookup"><span data-stu-id="17265-123">FromDate</span></span>](fromdate.md) <br/> |<span data-ttu-id="17265-124">Spécifie la date à laquelle le message a été envoyé.</span><span class="sxs-lookup"><span data-stu-id="17265-124">Specifies the date that the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="17265-125">ToDate</span><span class="sxs-lookup"><span data-stu-id="17265-125">ToDate</span></span>](todate.md) <br/> |<span data-ttu-id="17265-126">Spécifie la date à laquelle le message a été reçu.</span><span class="sxs-lookup"><span data-stu-id="17265-126">Specifies the date that the message was received.</span></span>  <br/> |
|[<span data-ttu-id="17265-127">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="17265-127">MessageTypes</span></span>](messagetypes.md) <br/> |<span data-ttu-id="17265-128">Spécifie un tableau de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="17265-128">Specifies an array of messages to search.</span></span>  <br/> |
|[<span data-ttu-id="17265-129">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="17265-129">SearchDumpster</span></span>](searchdumpster.md) <br/> |<span data-ttu-id="17265-130">Spécifie s’il faut rechercher dans les éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="17265-130">Specifies whether to search in deleted items.</span></span>  <br/> |
|[<span data-ttu-id="17265-131">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="17265-131">IncludePersonalArchive</span></span>](includepersonalarchive.md) <br/> |<span data-ttu-id="17265-132">Spécifie s’il faut inclure l’archive personnelle dans la recherche.</span><span class="sxs-lookup"><span data-stu-id="17265-132">Specifies whether to include the personal archive in the search.</span></span>  <br/> |
|[<span data-ttu-id="17265-133">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="17265-133">IncludeUnsearchableItems</span></span>](includeunsearchableitems.md) <br/> |<span data-ttu-id="17265-134">Spécifie s’il faut inclure des éléments qui ne peuvent pas être recherchés.</span><span class="sxs-lookup"><span data-stu-id="17265-134">Specifies whether to include items that cannot be searched.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17265-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="17265-135">Parent elements</span></span>

<span data-ttu-id="17265-136">Aucun.</span><span class="sxs-lookup"><span data-stu-id="17265-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17265-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="17265-137">Remarks</span></span>

<span data-ttu-id="17265-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="17265-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17265-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="17265-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17265-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="17265-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17265-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="17265-141">Schema Name</span></span>  <br/> |<span data-ttu-id="17265-142">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="17265-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="17265-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="17265-143">Validation File</span></span>  <br/> |<span data-ttu-id="17265-144">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="17265-144">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17265-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="17265-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="17265-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="17265-146">See also</span></span>



- [<span data-ttu-id="17265-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="17265-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

