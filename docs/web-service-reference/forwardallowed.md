---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: L’élément ForwardAllowed spécifie si les courriers électroniques de transfert sont activés.
ms.openlocfilehash: 3c722809bf68239c7d776108cb60d98afbed6e93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461932"
---
# <a name="forwardallowed"></a><span data-ttu-id="f3173-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="f3173-103">ForwardAllowed</span></span>

<span data-ttu-id="f3173-104">L’élément **ForwardAllowed** spécifie si les courriers électroniques de transfert sont activés.</span><span class="sxs-lookup"><span data-stu-id="f3173-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="f3173-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f3173-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3173-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3173-106">Attributes and elements</span></span>

<span data-ttu-id="f3173-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3173-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3173-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3173-108">Attributes</span></span>

<span data-ttu-id="f3173-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f3173-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3173-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3173-110">Child elements</span></span>

<span data-ttu-id="f3173-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3173-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3173-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3173-112">Parent elements</span></span>

|<span data-ttu-id="f3173-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f3173-113">**Element**</span></span>|<span data-ttu-id="f3173-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f3173-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3173-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="f3173-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="f3173-116">Spécifie les informations relatives à la licence de gestion des droits.</span><span class="sxs-lookup"><span data-stu-id="f3173-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3173-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f3173-117">Text value</span></span>

<span data-ttu-id="f3173-118">Une valeur de texte de **true** pour l’élément **ForwardAllowed** indique que le transfert de courriers électroniques est autorisé.</span><span class="sxs-lookup"><span data-stu-id="f3173-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="f3173-119">La valeur **false** indique que le transfert n’est pas autorisé.</span><span class="sxs-lookup"><span data-stu-id="f3173-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f3173-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="f3173-120">Remarks</span></span>

<span data-ttu-id="f3173-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f3173-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f3173-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3173-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3173-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3173-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3173-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3173-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3173-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3173-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f3173-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="f3173-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f3173-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="f3173-127">Validation File</span></span>  <br/> |<span data-ttu-id="f3173-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="f3173-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3173-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3173-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f3173-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f3173-130">See also</span></span>



- [<span data-ttu-id="f3173-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f3173-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

