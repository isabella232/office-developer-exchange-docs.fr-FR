---
title: ModifyRecipientsAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f25e673-0df0-4285-bf03-a083a395cdab
description: L’élément ModifyRecipientsAllowed spécifie si la modification des destinataires est activée.
ms.openlocfilehash: 3154ec3aceb2da7911002d505e0c452bf920d71f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465694"
---
# <a name="modifyrecipientsallowed"></a><span data-ttu-id="7c5a4-103">ModifyRecipientsAllowed</span><span class="sxs-lookup"><span data-stu-id="7c5a4-103">ModifyRecipientsAllowed</span></span>

<span data-ttu-id="7c5a4-104">L’élément **ModifyRecipientsAllowed** spécifie si la modification des destinataires est activée.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-104">The **ModifyRecipientsAllowed** element specifies whether modification of the recipients is enabled.</span></span> 
  
```XML
<ModifyRecipientsAllowed> true | false </ModifyRecipientsAllowed>
```

 <span data-ttu-id="7c5a4-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="7c5a4-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c5a4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7c5a4-106">Attributes and elements</span></span>

<span data-ttu-id="7c5a4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c5a4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7c5a4-108">Attributes</span></span>

<span data-ttu-id="7c5a4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c5a4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7c5a4-110">Child elements</span></span>

<span data-ttu-id="7c5a4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c5a4-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7c5a4-112">Parent elements</span></span>

[<span data-ttu-id="7c5a4-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="7c5a4-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="7c5a4-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7c5a4-114">Text value</span></span>

<span data-ttu-id="7c5a4-115">Une valeur de texte de **true** pour l’élément **ModifyRecipientsAllowed** indique que la liste de destinataires d’élément est modifiable pour un élément sur lequel la gestion des droits est activée.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-115">A text value of **true** for the **ModifyRecipientsAllowed** element indicates that the item recipient list is modifiable for an item with rights management enabled on it.</span></span> <span data-ttu-id="7c5a4-116">La valeur **false** indique que la liste des destinataires n’est pas modifiable.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-116">A value of **false** indicates that the recipient list is not modifiable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7c5a4-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="7c5a4-117">Remarks</span></span>

<span data-ttu-id="7c5a4-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c5a4-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c5a4-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c5a4-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7c5a4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c5a4-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7c5a4-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c5a4-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7c5a4-122">Schema name</span></span>  <br/> |<span data-ttu-id="7c5a4-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7c5a4-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c5a4-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7c5a4-124">Validation file</span></span>  <br/> |<span data-ttu-id="7c5a4-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c5a4-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c5a4-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7c5a4-126">Can be empty</span></span>  <br/> ||
   

