---
title: BeginTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2a60c89c-9c21-4041-9593-b244ac1608ef
description: L’élément BeginTime spécifie le début de la période de recherche des rappels.
ms.openlocfilehash: 4f926b8e4931c187cd4d5b97d6182d609bc15a1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463376"
---
# <a name="begintime"></a><span data-ttu-id="576e3-103">BeginTime</span><span class="sxs-lookup"><span data-stu-id="576e3-103">BeginTime</span></span>

<span data-ttu-id="576e3-104">L’élément **BeginTime** spécifie le début de la période de recherche des rappels.</span><span class="sxs-lookup"><span data-stu-id="576e3-104">The **BeginTime** element specifies the beginning of the time span to query for reminders.</span></span> 
  
```XML
<BeginTime/>
```

 <span data-ttu-id="576e3-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="576e3-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="576e3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="576e3-106">Attributes and elements</span></span>

<span data-ttu-id="576e3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="576e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="576e3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="576e3-108">Attributes</span></span>

<span data-ttu-id="576e3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="576e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="576e3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="576e3-110">Child elements</span></span>

<span data-ttu-id="576e3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="576e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="576e3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="576e3-112">Parent elements</span></span>

[<span data-ttu-id="576e3-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="576e3-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="576e3-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="576e3-114">Text value</span></span>

<span data-ttu-id="576e3-115">La valeur de texte de l’élément **BeginTime** correspond à l’heure de début de l’élément auquel la relance est destinée.</span><span class="sxs-lookup"><span data-stu-id="576e3-115">The text value of the **BeginTime** element is the beginning time of the item the reminder is for.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="576e3-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="576e3-116">Remarks</span></span>

<span data-ttu-id="576e3-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="576e3-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="576e3-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="576e3-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="576e3-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="576e3-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="576e3-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="576e3-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="576e3-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="576e3-121">Schema Name</span></span>  <br/> |<span data-ttu-id="576e3-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="576e3-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="576e3-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="576e3-123">Validation File</span></span>  <br/> |<span data-ttu-id="576e3-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="576e3-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="576e3-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="576e3-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="576e3-126">False</span><span class="sxs-lookup"><span data-stu-id="576e3-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="576e3-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="576e3-127">See also</span></span>



[<span data-ttu-id="576e3-128">GetReminders</span><span class="sxs-lookup"><span data-stu-id="576e3-128">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="576e3-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="576e3-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

