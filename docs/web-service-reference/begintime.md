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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463376"
---
# <a name="begintime"></a><span data-ttu-id="caacb-103">BeginTime</span><span class="sxs-lookup"><span data-stu-id="caacb-103">BeginTime</span></span>

<span data-ttu-id="caacb-104">L’élément **BeginTime** spécifie le début de la période de recherche des rappels.</span><span class="sxs-lookup"><span data-stu-id="caacb-104">The **BeginTime** element specifies the beginning of the time span to query for reminders.</span></span> 
  
```XML
<BeginTime/>
```

 <span data-ttu-id="caacb-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="caacb-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="caacb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="caacb-106">Attributes and elements</span></span>

<span data-ttu-id="caacb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="caacb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="caacb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="caacb-108">Attributes</span></span>

<span data-ttu-id="caacb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="caacb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="caacb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="caacb-110">Child elements</span></span>

<span data-ttu-id="caacb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="caacb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="caacb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="caacb-112">Parent elements</span></span>

[<span data-ttu-id="caacb-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="caacb-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="caacb-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="caacb-114">Text value</span></span>

<span data-ttu-id="caacb-115">La valeur de texte de l’élément **BeginTime** correspond à l’heure de début de l’élément auquel la relance est destinée.</span><span class="sxs-lookup"><span data-stu-id="caacb-115">The text value of the **BeginTime** element is the beginning time of the item the reminder is for.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="caacb-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="caacb-116">Remarks</span></span>

<span data-ttu-id="caacb-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="caacb-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="caacb-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="caacb-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="caacb-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="caacb-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="caacb-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="caacb-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="caacb-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="caacb-121">Schema Name</span></span>  <br/> |<span data-ttu-id="caacb-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="caacb-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="caacb-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="caacb-123">Validation File</span></span>  <br/> |<span data-ttu-id="caacb-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="caacb-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="caacb-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="caacb-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="caacb-126">False</span><span class="sxs-lookup"><span data-stu-id="caacb-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="caacb-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="caacb-127">See also</span></span>



[<span data-ttu-id="caacb-128">GetReminders</span><span class="sxs-lookup"><span data-stu-id="caacb-128">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="caacb-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="caacb-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

