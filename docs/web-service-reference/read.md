---
title: Lecture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Read
api_type:
- schema
ms.assetid: b14637e9-1695-4b7e-b078-ae527c2e4303
description: L’élément Read indique si un client peut lire un dossier ou un élément. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d75285e0ab14c4f53d73cb7f4349196e07c3c521
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468312"
---
# <a name="read"></a><span data-ttu-id="596c5-104">Lecture</span><span class="sxs-lookup"><span data-stu-id="596c5-104">Read</span></span>

<span data-ttu-id="596c5-105">L’élément **Read** indique si un client peut lire un dossier ou un élément.</span><span class="sxs-lookup"><span data-stu-id="596c5-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="596c5-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="596c5-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="596c5-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="596c5-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="596c5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="596c5-108">Attributes and elements</span></span>

<span data-ttu-id="596c5-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="596c5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="596c5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="596c5-110">Attributes</span></span>

<span data-ttu-id="596c5-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="596c5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="596c5-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="596c5-112">Child elements</span></span>

<span data-ttu-id="596c5-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="596c5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="596c5-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="596c5-114">Parent elements</span></span>

|<span data-ttu-id="596c5-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="596c5-115">**Element**</span></span>|<span data-ttu-id="596c5-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="596c5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="596c5-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="596c5-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="596c5-118">Contient les droits du client en fonction des paramètres d’autorisation de l’élément ou du dossier.</span><span class="sxs-lookup"><span data-stu-id="596c5-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="596c5-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="596c5-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="596c5-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="596c5-120">Text value</span></span>

<span data-ttu-id="596c5-121">Une valeur de texte **true** indique qu’un client peut lire un élément de dossier.</span><span class="sxs-lookup"><span data-stu-id="596c5-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="596c5-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="596c5-122">Remarks</span></span>

<span data-ttu-id="596c5-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="596c5-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="596c5-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="596c5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="596c5-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="596c5-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="596c5-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="596c5-126">Schema Name</span></span>  <br/> |<span data-ttu-id="596c5-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="596c5-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="596c5-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="596c5-128">Validation File</span></span>  <br/> |<span data-ttu-id="596c5-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="596c5-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="596c5-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="596c5-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="596c5-131">False</span><span class="sxs-lookup"><span data-stu-id="596c5-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="596c5-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="596c5-132">See also</span></span>



- [<span data-ttu-id="596c5-133">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="596c5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="596c5-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="596c5-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

