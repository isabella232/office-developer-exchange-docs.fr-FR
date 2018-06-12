---
title: Modifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Modify
api_type:
- schema
ms.assetid: 7a51e9e1-addb-4343-8a22-78f23763c0a8
description: L’élément modifier indique si un client peut modifier un dossier ou un élément. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 29fd2184e83f66a9b7e7db4173a765cee2922be8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828514"
---
# <a name="modify"></a><span data-ttu-id="18f67-104">Modifier</span><span class="sxs-lookup"><span data-stu-id="18f67-104">Modify</span></span>

<span data-ttu-id="18f67-105">L’élément **Modifier** indique si un client peut modifier un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="18f67-105">The **Modify** element indicates whether a client can modify a folder or item.</span></span> <span data-ttu-id="18f67-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="18f67-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Modify>true or false</Modify>
```

 <span data-ttu-id="18f67-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="18f67-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18f67-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="18f67-108">Attributes and elements</span></span>

<span data-ttu-id="18f67-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="18f67-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18f67-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="18f67-110">Attributes</span></span>

<span data-ttu-id="18f67-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18f67-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18f67-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="18f67-112">Child elements</span></span>

<span data-ttu-id="18f67-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="18f67-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18f67-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="18f67-114">Parent elements</span></span>

|<span data-ttu-id="18f67-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="18f67-115">**Element**</span></span>|<span data-ttu-id="18f67-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="18f67-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18f67-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="18f67-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="18f67-118">Contient les droits du client en fonction des paramètres d’autorisation pour l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="18f67-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="18f67-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="18f67-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18f67-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="18f67-120">Text value</span></span>

<span data-ttu-id="18f67-121">Une valeur de texte de **la valeur true** indique qu’un client peut modifier un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="18f67-121">A text value of **true** indicates that a client can modify an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="18f67-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="18f67-122">Remarks</span></span>

<span data-ttu-id="18f67-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="18f67-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18f67-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="18f67-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18f67-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="18f67-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18f67-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="18f67-126">Schema Name</span></span>  <br/> |<span data-ttu-id="18f67-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="18f67-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="18f67-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="18f67-128">Validation File</span></span>  <br/> |<span data-ttu-id="18f67-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18f67-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18f67-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="18f67-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="18f67-131">False</span><span class="sxs-lookup"><span data-stu-id="18f67-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18f67-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="18f67-132">See also</span></span>



- [<span data-ttu-id="18f67-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="18f67-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="18f67-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="18f67-134">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)
