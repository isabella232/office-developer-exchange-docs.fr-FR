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
description: L’élément IsModerated indique si la boîte aux lettres du destinataire est en cours modéré.
ms.openlocfilehash: 8db234f9706bb8187978a76f745323749d7a640a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828055"
---
# <a name="ismoderated"></a><span data-ttu-id="37faa-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="37faa-103">IsModerated</span></span>

<span data-ttu-id="37faa-104">L’élément **IsModerated** indique si la boîte aux lettres du destinataire est en cours modéré.</span><span class="sxs-lookup"><span data-stu-id="37faa-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="37faa-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="37faa-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37faa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="37faa-106">Attributes and elements</span></span>

<span data-ttu-id="37faa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="37faa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37faa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="37faa-108">Attributes</span></span>

<span data-ttu-id="37faa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37faa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37faa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="37faa-110">Child elements</span></span>

<span data-ttu-id="37faa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37faa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37faa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="37faa-112">Parent elements</span></span>

|<span data-ttu-id="37faa-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37faa-113">**Element**</span></span>|<span data-ttu-id="37faa-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="37faa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37faa-115">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="37faa-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="37faa-116">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="37faa-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37faa-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="37faa-117">Text value</span></span>

<span data-ttu-id="37faa-118">La valeur de texte pour cet élément est **la valeur true** si la boîte aux lettres du destinataire est modéré.</span><span class="sxs-lookup"><span data-stu-id="37faa-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="37faa-119">La valeur est **false** si la boîte aux lettres du destinataire n’est pas en cours modéré.</span><span class="sxs-lookup"><span data-stu-id="37faa-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="37faa-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="37faa-120">Remarks</span></span>

<span data-ttu-id="37faa-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="37faa-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37faa-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="37faa-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37faa-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="37faa-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37faa-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="37faa-124">Schema Name</span></span>  <br/> |<span data-ttu-id="37faa-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="37faa-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="37faa-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="37faa-126">Validation File</span></span>  <br/> |<span data-ttu-id="37faa-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="37faa-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37faa-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="37faa-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="37faa-129">False</span><span class="sxs-lookup"><span data-stu-id="37faa-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37faa-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="37faa-130">See also</span></span>



- [<span data-ttu-id="37faa-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="37faa-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

