---
title: ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: affe84a5-ad98-4aba-83f4-8732938b763d
description: L’élément ExpandDL définit une demande de développement d’une liste de distribution.
ms.openlocfilehash: 52b1ea1b51ce185c7a266e3002a4484e4b813bc0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456933"
---
# <a name="expanddl"></a><span data-ttu-id="80a5e-103">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="80a5e-103">ExpandDL</span></span>

<span data-ttu-id="80a5e-104">L’élément **ExpandDL** définit une demande de développement d’une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="80a5e-104">The **ExpandDL** element defines a request to expand a distribution list.</span></span> 
  
```xml
<ExpandDL>
   <Mailbox/>
</ExpandDL>
```

 <span data-ttu-id="80a5e-105">**ExpandDLType**</span><span class="sxs-lookup"><span data-stu-id="80a5e-105">**ExpandDLType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80a5e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="80a5e-106">Attributes and elements</span></span>

<span data-ttu-id="80a5e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="80a5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80a5e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="80a5e-108">Attributes</span></span>

<span data-ttu-id="80a5e-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="80a5e-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80a5e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="80a5e-110">Child elements</span></span>

|<span data-ttu-id="80a5e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="80a5e-111">**Element**</span></span>|<span data-ttu-id="80a5e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="80a5e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80a5e-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="80a5e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="80a5e-114">Identifie une adresse de messagerie entièrement résolue ou une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="80a5e-114">Identifies a fully resolved e-mail address or a distribution list.</span></span> <span data-ttu-id="80a5e-115">Cette boîte aux lettres représente la liste de distribution à développer.</span><span class="sxs-lookup"><span data-stu-id="80a5e-115">This mailbox represents the distribution list to expand.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80a5e-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="80a5e-116">Parent elements</span></span>

<span data-ttu-id="80a5e-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="80a5e-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80a5e-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="80a5e-118">Remarks</span></span>

<span data-ttu-id="80a5e-119">Une extension de liste de distribution est effectuée uniquement pour une seule liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="80a5e-119">A distribution list expansion will only be performed for a single distribution list.</span></span> <span data-ttu-id="80a5e-120">Le développement d’une liste de distribution n’est pas récursif.</span><span class="sxs-lookup"><span data-stu-id="80a5e-120">A distribution list expansion is not recursive.</span></span>
  
<span data-ttu-id="80a5e-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="80a5e-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80a5e-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="80a5e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80a5e-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="80a5e-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="80a5e-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="80a5e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="80a5e-125">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="80a5e-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="80a5e-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="80a5e-126">Validation File</span></span>  <br/> |<span data-ttu-id="80a5e-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="80a5e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="80a5e-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="80a5e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="80a5e-129">False</span><span class="sxs-lookup"><span data-stu-id="80a5e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80a5e-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="80a5e-130">See also</span></span>



[<span data-ttu-id="80a5e-131">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="80a5e-131">ExpandDL operation</span></span>](expanddl-operation.md)

