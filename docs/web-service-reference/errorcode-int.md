---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: L’élément ErrorCode spécifie le code d’erreur d’une recherche ayant échoué effectuée dans une boîte aux lettres.
ms.openlocfilehash: 24170a56e5fa23c3811fcbd27f0240e6ba3c87b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460665"
---
# <a name="errorcode-int"></a><span data-ttu-id="3cf15-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="3cf15-103">ErrorCode (int)</span></span>

<span data-ttu-id="3cf15-104">L’élément **ErrorCode** spécifie le code d’erreur d’une recherche ayant échoué effectuée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3cf15-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="3cf15-105">**int**</span><span class="sxs-lookup"><span data-stu-id="3cf15-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cf15-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3cf15-106">Attributes and elements</span></span>

<span data-ttu-id="3cf15-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3cf15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cf15-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3cf15-108">Attributes</span></span>

<span data-ttu-id="3cf15-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3cf15-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cf15-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3cf15-110">Child elements</span></span>

<span data-ttu-id="3cf15-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3cf15-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3cf15-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3cf15-112">Parent elements</span></span>

|<span data-ttu-id="3cf15-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3cf15-113">**Element**</span></span>|<span data-ttu-id="3cf15-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3cf15-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cf15-115">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="3cf15-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="3cf15-116">Spécifie l’état de conservation de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3cf15-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3cf15-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3cf15-117">Text value</span></span>

<span data-ttu-id="3cf15-118">La valeur de texte de l’élément **ErrorCode** est le code d’erreur renvoyé pour une recherche ayant échoué dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3cf15-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3cf15-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="3cf15-119">Remarks</span></span>

<span data-ttu-id="3cf15-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3cf15-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3cf15-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3cf15-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3cf15-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3cf15-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cf15-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3cf15-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cf15-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3cf15-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3cf15-125">Schéma type</span><span class="sxs-lookup"><span data-stu-id="3cf15-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="3cf15-126">Validation File</span><span class="sxs-lookup"><span data-stu-id="3cf15-126">Validation File</span></span>  <br/> |<span data-ttu-id="3cf15-127">types. xsd</span><span class="sxs-lookup"><span data-stu-id="3cf15-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cf15-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3cf15-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3cf15-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3cf15-129">See also</span></span>



- [<span data-ttu-id="3cf15-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3cf15-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

