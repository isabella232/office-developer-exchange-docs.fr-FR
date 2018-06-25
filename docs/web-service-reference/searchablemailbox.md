---
title: SearchableMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 339005cd-a3b9-47dd-bc7b-a860b699625b
description: L’élément SearchableMailbox spécifie une boîte aux lettres renvoyé à partir d’une demande GetSearchableMailboxes.
ms.openlocfilehash: 0d0981d050fa388e83eaa8408b60d305296c1f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829284"
---
# <a name="searchablemailbox"></a><span data-ttu-id="5607a-103">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="5607a-103">SearchableMailbox</span></span>

<span data-ttu-id="5607a-104">L’élément **SearchableMailbox** spécifie une boîte aux lettres renvoyé à partir d’une demande **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="5607a-104">The **SearchableMailbox** element specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<SearchableMailbox>
   <Guid/>
   <PrimarySmtpAddress/>
   <IsExternalMailbox/>
   <ExternalEmailAddress/>
   <DisplayName/>
   <IsMembershipGroup/>
   <ReferenceId/>
</SearchableMailbox>
```

 <span data-ttu-id="5607a-105">**SearchableMailboxType**</span><span class="sxs-lookup"><span data-stu-id="5607a-105">**SearchableMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5607a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5607a-106">Attributes and elements</span></span>

<span data-ttu-id="5607a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5607a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5607a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5607a-108">Attributes</span></span>

<span data-ttu-id="5607a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5607a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5607a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5607a-110">Child elements</span></span>

<span data-ttu-id="5607a-111">[GUID](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md)  |  [ ReferenceId](referenceid.md)</span><span class="sxs-lookup"><span data-stu-id="5607a-111">[Guid](guid-ex15websvcsotherref.md) | [PrimarySmtpAddress (string)](primarysmtpaddress-string.md) | [IsExternalMailbox](isexternalmailbox.md) | [ExternalEmailAddress](externalemailaddress.md) | [DisplayName (string)](displayname-string.md) | [IsMembershipGroup](ismembershipgroup.md) | [ReferenceId](referenceid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5607a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5607a-112">Parent elements</span></span>

[<span data-ttu-id="5607a-113">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="5607a-113">SearchableMailboxes</span></span>](searchablemailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="5607a-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="5607a-114">Remarks</span></span>

<span data-ttu-id="5607a-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5607a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5607a-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5607a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5607a-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5607a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5607a-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5607a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5607a-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5607a-119">Schema name</span></span>  <br/> |<span data-ttu-id="5607a-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5607a-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="5607a-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5607a-121">Validation file</span></span>  <br/> |<span data-ttu-id="5607a-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5607a-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5607a-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5607a-123">Can be empty</span></span>  <br/> ||
   

