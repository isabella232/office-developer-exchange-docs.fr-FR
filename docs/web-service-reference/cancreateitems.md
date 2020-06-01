---
title: CanCreateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanCreateItems
api_type:
- schema
ms.assetid: c4574e9a-3c42-40a1-a5f9-79b6560e9b30
description: L’élément CanCreateItems indique si un utilisateur est autorisé à créer des éléments dans un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 73d3d967774d9fcff53722d0936462025e02b659
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458781"
---
# <a name="cancreateitems"></a><span data-ttu-id="186b5-104">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="186b5-104">CanCreateItems</span></span>

<span data-ttu-id="186b5-105">L’élément **CanCreateItems** indique si un utilisateur est autorisé à créer des éléments dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="186b5-105">The **CanCreateItems** element indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="186b5-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="186b5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CanCreateItems/>
```

 <span data-ttu-id="186b5-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="186b5-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="186b5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="186b5-108">Attributes and elements</span></span>

<span data-ttu-id="186b5-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="186b5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="186b5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="186b5-110">Attributes</span></span>

<span data-ttu-id="186b5-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="186b5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="186b5-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="186b5-112">Child elements</span></span>

<span data-ttu-id="186b5-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="186b5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="186b5-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="186b5-114">Parent elements</span></span>

|<span data-ttu-id="186b5-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="186b5-115">**Element**</span></span>|<span data-ttu-id="186b5-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="186b5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="186b5-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="186b5-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="186b5-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="186b5-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="186b5-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="186b5-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="186b5-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="186b5-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="186b5-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="186b5-123">Text value</span></span>

<span data-ttu-id="186b5-124">Une valeur de texte **true** indique que l’utilisateur peut créer des éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="186b5-124">A text value of **true** indicates that the user can create items in the folder.</span></span> <span data-ttu-id="186b5-125">La valeur **false** indique que l’utilisateur ne peut pas créer d’éléments dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="186b5-125">A value of **false** indicates that the user cannot create items in the folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="186b5-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="186b5-126">Remarks</span></span>

<span data-ttu-id="186b5-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="186b5-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="186b5-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="186b5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="186b5-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="186b5-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="186b5-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="186b5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="186b5-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="186b5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="186b5-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="186b5-132">Validation File</span></span>  <br/> |<span data-ttu-id="186b5-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="186b5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="186b5-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="186b5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="186b5-135">False</span><span class="sxs-lookup"><span data-stu-id="186b5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="186b5-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="186b5-136">See also</span></span>



- [<span data-ttu-id="186b5-137">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="186b5-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="186b5-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="186b5-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

