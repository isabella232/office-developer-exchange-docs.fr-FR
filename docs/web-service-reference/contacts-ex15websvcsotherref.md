---
title: Contacts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contacts
api_type:
- schema
ms.assetid: 0cc67cdf-9707-45e7-92c6-fa83a016cdbe
description: L’élément de Contacts contient une liste des contacts qui sont associés à une tâche.
ms.openlocfilehash: da7963d30f58f7da52e76e3f7f1d0f7fd68abf74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755556"
---
# <a name="contacts"></a><span data-ttu-id="26a2e-103">Contacts</span><span class="sxs-lookup"><span data-stu-id="26a2e-103">Contacts</span></span>

<span data-ttu-id="26a2e-104">L’élément de **Contacts** contient une liste des contacts qui sont associés à une tâche.</span><span class="sxs-lookup"><span data-stu-id="26a2e-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="26a2e-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="26a2e-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26a2e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="26a2e-106">Attributes and elements</span></span>

<span data-ttu-id="26a2e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="26a2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26a2e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="26a2e-108">Attributes</span></span>

<span data-ttu-id="26a2e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="26a2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26a2e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="26a2e-110">Child elements</span></span>

|<span data-ttu-id="26a2e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="26a2e-111">**Element**</span></span>|<span data-ttu-id="26a2e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="26a2e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26a2e-113">String</span><span class="sxs-lookup"><span data-stu-id="26a2e-113">String</span></span>](string.md) <br/> |<span data-ttu-id="26a2e-114">Représente une liste séparée par des virgules des noms de contacts.</span><span class="sxs-lookup"><span data-stu-id="26a2e-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26a2e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="26a2e-115">Parent elements</span></span>

|<span data-ttu-id="26a2e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="26a2e-116">**Element**</span></span>|<span data-ttu-id="26a2e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="26a2e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26a2e-118">Tâche</span><span class="sxs-lookup"><span data-stu-id="26a2e-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="26a2e-119">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="26a2e-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26a2e-120">Note</span><span class="sxs-lookup"><span data-stu-id="26a2e-120">Remarks</span></span>

<span data-ttu-id="26a2e-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="26a2e-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26a2e-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="26a2e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26a2e-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="26a2e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26a2e-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="26a2e-124">Schema name</span></span>  <br/> |<span data-ttu-id="26a2e-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="26a2e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="26a2e-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="26a2e-126">Validation file</span></span>  <br/> |<span data-ttu-id="26a2e-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="26a2e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26a2e-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="26a2e-128">Can be empty</span></span>  <br/> |<span data-ttu-id="26a2e-129">False</span><span class="sxs-lookup"><span data-stu-id="26a2e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26a2e-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="26a2e-130">See also</span></span>



- [<span data-ttu-id="26a2e-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="26a2e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

