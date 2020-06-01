---
title: Nom (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: 98c58c53-9acc-4e89-9fcf-03f1b05abee1
description: L’élément Name représente le nom d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: db6eb547b5c848dc31bbaa377692989b16771673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466926"
---
# <a name="name-emailaddresstype"></a><span data-ttu-id="844ac-103">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="844ac-103">Name (EmailAddressType)</span></span>

<span data-ttu-id="844ac-104">L’élément **Name** représente le nom d’un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="844ac-104">The **Name** element represents the name of a mailbox user.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="844ac-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="844ac-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="844ac-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="844ac-106">Attributes and elements</span></span>

<span data-ttu-id="844ac-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="844ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="844ac-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="844ac-108">Attributes</span></span>

<span data-ttu-id="844ac-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="844ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="844ac-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="844ac-110">Child elements</span></span>

<span data-ttu-id="844ac-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="844ac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="844ac-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="844ac-112">Parent elements</span></span>

|<span data-ttu-id="844ac-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="844ac-113">**Element**</span></span>|<span data-ttu-id="844ac-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="844ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="844ac-115">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="844ac-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="844ac-116">Identifie une adresse de messagerie entièrement résolue.</span><span class="sxs-lookup"><span data-stu-id="844ac-116">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="844ac-117">RoomList</span><span class="sxs-lookup"><span data-stu-id="844ac-117">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="844ac-118">Identifie une liste de salles de réunion.</span><span class="sxs-lookup"><span data-stu-id="844ac-118">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="844ac-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="844ac-119">Text value</span></span>

<span data-ttu-id="844ac-120">Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="844ac-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="844ac-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="844ac-121">Remarks</span></span>

<span data-ttu-id="844ac-122">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="844ac-122">This element is optional.</span></span> <span data-ttu-id="844ac-123">L’élément **Name** existe dans les types **AttachmentType**, **EmailAddressType**et **EmailAddress** .</span><span class="sxs-lookup"><span data-stu-id="844ac-123">The **Name** element exists in the **AttachmentType**, **EmailAddressType**, and **EmailAddress** types.</span></span> <span data-ttu-id="844ac-124">L’élément **Name** dans le type **EmailAddress** est décrit dans la rubrique de l’élément [Name (EmailAddress)](name-emailaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="844ac-124">The **Name** element in the **EmailAddress** type is described in the [Name (EmailAddress)](name-emailaddress.md) element topic.</span></span> 
  
<span data-ttu-id="844ac-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="844ac-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="844ac-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="844ac-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="844ac-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="844ac-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="844ac-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="844ac-128">Schema Name</span></span>  <br/> |<span data-ttu-id="844ac-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="844ac-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="844ac-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="844ac-130">Validation File</span></span>  <br/> |<span data-ttu-id="844ac-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="844ac-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="844ac-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="844ac-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="844ac-133">False</span><span class="sxs-lookup"><span data-stu-id="844ac-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="844ac-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="844ac-134">See also</span></span>

- [<span data-ttu-id="844ac-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="844ac-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

