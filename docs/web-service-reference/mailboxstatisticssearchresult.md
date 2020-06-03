---
title: MailboxStatisticsSearchResult
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 73499df7-3d50-4e39-895d-6e15dd8b2777
description: L’élément MailboxStatisticsSearchResult contient les résultats d’une recherche par mot clé.
ms.openlocfilehash: c300c6c2ec9ab3c772709edd3e6a1c7fea19d6e3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44440847"
---
# <a name="mailboxstatisticssearchresult"></a><span data-ttu-id="26a08-103">MailboxStatisticsSearchResult</span><span class="sxs-lookup"><span data-stu-id="26a08-103">MailboxStatisticsSearchResult</span></span>

<span data-ttu-id="26a08-104">L’élément **MailboxStatisticsSearchResult** contient les résultats d’une recherche par mot clé.</span><span class="sxs-lookup"><span data-stu-id="26a08-104">The **MailboxStatisticsSearchResult** element contains the results of a keyword search.</span></span> 
  
```XML
<MailboxStatisticsSearchResult>
   <UserMailbox/>
   <KeywordStatisticsSearchResult/>
</MailboxStatisticsSearchResult>
```

<span data-ttu-id="26a08-105">**MailboxStatisticsSearchResultType**</span><span class="sxs-lookup"><span data-stu-id="26a08-105">**MailboxStatisticsSearchResultType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="26a08-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="26a08-106">Attributes and elements</span></span>

<span data-ttu-id="26a08-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="26a08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26a08-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="26a08-108">Attributes</span></span>

<span data-ttu-id="26a08-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="26a08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26a08-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="26a08-110">Child elements</span></span>

<span data-ttu-id="26a08-111">[UserMailbox](usermailbox.md)  |  [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="26a08-111">[UserMailbox](usermailbox.md) | [KeywordStatisticsSearchResult](keywordstatisticssearchresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26a08-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="26a08-112">Parent elements</span></span>

[<span data-ttu-id="26a08-113">FindMailboxStatisticsByKeywordsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="26a08-113">FindMailboxStatisticsByKeywordsResponseMessage</span></span>](findmailboxstatisticsbykeywordsresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="26a08-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="26a08-114">Remarks</span></span>

<span data-ttu-id="26a08-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="26a08-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26a08-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="26a08-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26a08-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="26a08-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26a08-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="26a08-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26a08-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="26a08-119">Schema name</span></span>  <br/> |<span data-ttu-id="26a08-120">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="26a08-120">messages schema</span></span>  <br/> |
|<span data-ttu-id="26a08-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="26a08-121">Validation file</span></span>  <br/> |<span data-ttu-id="26a08-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="26a08-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26a08-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="26a08-123">Can be empty</span></span>  <br/> ||
   

