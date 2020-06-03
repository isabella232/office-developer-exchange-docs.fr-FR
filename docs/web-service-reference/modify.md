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
description: L’élément Modify indique si un client peut modifier un dossier ou un élément. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e7712644ac9c32afab06be49b438ad83bbb31058
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530414"
---
# <a name="modify"></a><span data-ttu-id="16b56-104">Modifier</span><span class="sxs-lookup"><span data-stu-id="16b56-104">Modify</span></span>

<span data-ttu-id="16b56-105">L’élément **Modify** indique si un client peut modifier un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="16b56-105">The **Modify** element indicates whether a client can modify a folder or item.</span></span> <span data-ttu-id="16b56-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="16b56-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Modify>true or false</Modify>
```

 <span data-ttu-id="16b56-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="16b56-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16b56-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="16b56-108">Attributes and elements</span></span>

<span data-ttu-id="16b56-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="16b56-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16b56-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="16b56-110">Attributes</span></span>

<span data-ttu-id="16b56-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="16b56-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16b56-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="16b56-112">Child elements</span></span>

<span data-ttu-id="16b56-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="16b56-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16b56-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="16b56-114">Parent elements</span></span>

|<span data-ttu-id="16b56-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="16b56-115">**Element**</span></span>|<span data-ttu-id="16b56-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="16b56-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16b56-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="16b56-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="16b56-118">Contient les droits du client en fonction des paramètres d’autorisation de l’élément ou du dossier.</span><span class="sxs-lookup"><span data-stu-id="16b56-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="16b56-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="16b56-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="16b56-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="16b56-120">Text value</span></span>

<span data-ttu-id="16b56-121">Une valeur de texte **true** indique qu’un client peut modifier un élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="16b56-121">A text value of **true** indicates that a client can modify an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="16b56-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="16b56-122">Remarks</span></span>

<span data-ttu-id="16b56-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="16b56-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16b56-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="16b56-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16b56-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="16b56-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16b56-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="16b56-126">Schema Name</span></span>  <br/> |<span data-ttu-id="16b56-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="16b56-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="16b56-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="16b56-128">Validation File</span></span>  <br/> |<span data-ttu-id="16b56-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="16b56-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16b56-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="16b56-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="16b56-131">False</span><span class="sxs-lookup"><span data-stu-id="16b56-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16b56-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="16b56-132">See also</span></span>



- [<span data-ttu-id="16b56-133">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="16b56-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="16b56-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="16b56-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

