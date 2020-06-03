---
title: IsModerated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: L’élément IsModerated indique si la boîte aux lettres du destinataire est modéré.
ms.openlocfilehash: 930d5a7e09712f35d22850a93462d051a34785a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435484"
---
# <a name="ismoderated"></a><span data-ttu-id="c9902-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="c9902-103">IsModerated</span></span>

<span data-ttu-id="c9902-104">L’élément **IsModerated** indique si la boîte aux lettres du destinataire est modéré.</span><span class="sxs-lookup"><span data-stu-id="c9902-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="c9902-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c9902-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9902-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c9902-106">Attributes and elements</span></span>

<span data-ttu-id="c9902-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c9902-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9902-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c9902-108">Attributes</span></span>

<span data-ttu-id="c9902-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c9902-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9902-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c9902-110">Child elements</span></span>

<span data-ttu-id="c9902-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c9902-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c9902-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c9902-112">Parent elements</span></span>

|<span data-ttu-id="c9902-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c9902-113">**Element**</span></span>|<span data-ttu-id="c9902-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c9902-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9902-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="c9902-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="c9902-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="c9902-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9902-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c9902-117">Text value</span></span>

<span data-ttu-id="c9902-118">La valeur de texte de cet élément est **true** si la boîte aux lettres du destinataire est modérée.</span><span class="sxs-lookup"><span data-stu-id="c9902-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="c9902-119">La valeur est **false** si la boîte aux lettres du destinataire n’est pas modérée.</span><span class="sxs-lookup"><span data-stu-id="c9902-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c9902-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="c9902-120">Remarks</span></span>

<span data-ttu-id="c9902-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9902-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9902-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c9902-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9902-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c9902-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9902-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c9902-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c9902-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c9902-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9902-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c9902-126">Validation File</span></span>  <br/> |<span data-ttu-id="c9902-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c9902-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9902-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c9902-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9902-129">False</span><span class="sxs-lookup"><span data-stu-id="c9902-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9902-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c9902-130">See also</span></span>



- [<span data-ttu-id="c9902-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c9902-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

