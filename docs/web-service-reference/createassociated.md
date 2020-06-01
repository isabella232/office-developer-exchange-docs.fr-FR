---
title: CreateAssociated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: L’élément CreateAssociated indique si un client peut créer une table de contenu associée. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e88d7670fd9ef848221dab8cc145395bcb11e5bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460791"
---
# <a name="createassociated"></a><span data-ttu-id="ff736-104">CreateAssociated</span><span class="sxs-lookup"><span data-stu-id="ff736-104">CreateAssociated</span></span>

<span data-ttu-id="ff736-105">L’élément **CreateAssociated** indique si un client peut créer une table de contenu associée.</span><span class="sxs-lookup"><span data-stu-id="ff736-105">The **CreateAssociated** element indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="ff736-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ff736-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 <span data-ttu-id="ff736-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="ff736-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff736-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ff736-108">Attributes and elements</span></span>

<span data-ttu-id="ff736-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ff736-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff736-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ff736-110">Attributes</span></span>

<span data-ttu-id="ff736-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ff736-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff736-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ff736-112">Child elements</span></span>

<span data-ttu-id="ff736-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ff736-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff736-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ff736-114">Parent elements</span></span>

|<span data-ttu-id="ff736-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff736-115">**Element**</span></span>|<span data-ttu-id="ff736-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff736-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff736-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ff736-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ff736-118">Contient les droits du client en fonction des paramètres d’autorisation de l’élément ou du dossier.</span><span class="sxs-lookup"><span data-stu-id="ff736-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ff736-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ff736-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff736-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ff736-120">Text value</span></span>

<span data-ttu-id="ff736-121">Une valeur de texte **true** indique qu’un client peut créer une table de contenu associée.</span><span class="sxs-lookup"><span data-stu-id="ff736-121">A text value of **true** indicates that a client can create an associated contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ff736-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ff736-122">Remarks</span></span>

<span data-ttu-id="ff736-123">Cette propriété est utilisée uniquement sur les objets Folder.</span><span class="sxs-lookup"><span data-stu-id="ff736-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="ff736-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ff736-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff736-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ff736-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff736-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ff736-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff736-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ff736-127">Schema Name</span></span>  <br/> |<span data-ttu-id="ff736-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ff736-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff736-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ff736-129">Validation File</span></span>  <br/> |<span data-ttu-id="ff736-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ff736-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff736-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ff736-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff736-132">False</span><span class="sxs-lookup"><span data-stu-id="ff736-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff736-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff736-133">See also</span></span>



- [<span data-ttu-id="ff736-134">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ff736-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ff736-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="ff736-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

