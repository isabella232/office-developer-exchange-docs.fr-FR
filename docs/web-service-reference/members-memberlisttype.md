---
title: Membres (MemberListType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Members
api_type:
- schema
ms.assetid: cbd38049-2ef7-40bf-9bec-0469af0f58ec
description: L’élément membres fournit la liste des membres pour une liste de distribution.
ms.openlocfilehash: 8cf9ed7a64a908614ce7be30a9bef631739fcebf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828439"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="3b947-103">Membres (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="3b947-103">Members (MemberListType)</span></span>

<span data-ttu-id="3b947-104">L’élément **membres** fournit la liste des membres pour une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="3b947-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="3b947-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="3b947-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3b947-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3b947-106">Attributes and elements</span></span>

<span data-ttu-id="3b947-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3b947-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b947-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3b947-108">Attributes</span></span>

<span data-ttu-id="3b947-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3b947-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b947-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3b947-110">Child elements</span></span>

|<span data-ttu-id="3b947-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3b947-111">**Element**</span></span>|<span data-ttu-id="3b947-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3b947-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b947-113">Membre</span><span class="sxs-lookup"><span data-stu-id="3b947-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3b947-114">Fournit un identificateur pour une adresse de messagerie entièrement résolu et l’état de l’adresse sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="3b947-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="3b947-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="3b947-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b947-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3b947-116">Parent elements</span></span>

|<span data-ttu-id="3b947-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3b947-117">**Element**</span></span>|<span data-ttu-id="3b947-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="3b947-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b947-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="3b947-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3b947-120">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="3b947-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b947-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="3b947-121">Remarks</span></span>

<span data-ttu-id="3b947-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b947-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b947-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3b947-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b947-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3b947-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b947-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3b947-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3b947-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3b947-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b947-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3b947-127">Validation File</span></span>  <br/> |<span data-ttu-id="3b947-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b947-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b947-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3b947-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b947-130">False</span><span class="sxs-lookup"><span data-stu-id="3b947-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b947-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3b947-131">See also</span></span>

- [<span data-ttu-id="3b947-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3b947-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

