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
description: L’élément Members fournit la liste des membres d’une liste de distribution.
ms.openlocfilehash: 2cdfb81dfbc223db365d49ed44d4893339eb4653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462429"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="f8372-103">Membres (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="f8372-103">Members (MemberListType)</span></span>

<span data-ttu-id="f8372-104">L’élément **members** fournit la liste des membres d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="f8372-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="f8372-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="f8372-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f8372-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f8372-106">Attributes and elements</span></span>

<span data-ttu-id="f8372-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f8372-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8372-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f8372-108">Attributes</span></span>

<span data-ttu-id="f8372-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f8372-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8372-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f8372-110">Child elements</span></span>

|<span data-ttu-id="f8372-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8372-111">**Element**</span></span>|<span data-ttu-id="f8372-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8372-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8372-113">Membre</span><span class="sxs-lookup"><span data-stu-id="f8372-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f8372-114">Fournit un identificateur pour une adresse de messagerie entièrement résolue et l’état de cette adresse sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="f8372-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="f8372-115">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f8372-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8372-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f8372-116">Parent elements</span></span>

|<span data-ttu-id="f8372-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8372-117">**Element**</span></span>|<span data-ttu-id="f8372-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8372-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8372-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="f8372-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f8372-120">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="f8372-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8372-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="f8372-121">Remarks</span></span>

<span data-ttu-id="f8372-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8372-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8372-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f8372-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8372-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f8372-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8372-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f8372-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f8372-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f8372-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8372-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f8372-127">Validation File</span></span>  <br/> |<span data-ttu-id="f8372-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f8372-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8372-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f8372-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8372-130">False</span><span class="sxs-lookup"><span data-stu-id="f8372-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8372-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f8372-131">See also</span></span>

- [<span data-ttu-id="f8372-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f8372-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

