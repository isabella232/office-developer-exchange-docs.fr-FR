---
title: Diagnostics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: L’élément Diagnostics fournit des informations sur le temps et les performances utilisées pour la création de rapports dans un centre de données.
ms.openlocfilehash: 9eb46ef7ceb877372aff9b029190af8c8d8115cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467836"
---
# <a name="diagnostics"></a><span data-ttu-id="7b5df-103">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="7b5df-103">Diagnostics</span></span>

<span data-ttu-id="7b5df-104">L’élément **Diagnostics** fournit des informations sur le temps et les performances utilisées pour la création de rapports dans un centre de données.</span><span class="sxs-lookup"><span data-stu-id="7b5df-104">The **Diagnostics** element provides timing and performance information that is used for reporting in a DataCenter.</span></span> 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 <span data-ttu-id="7b5df-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="7b5df-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b5df-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b5df-106">Attributes and elements</span></span>

<span data-ttu-id="7b5df-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b5df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b5df-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b5df-108">Attributes</span></span>

<span data-ttu-id="7b5df-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b5df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b5df-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b5df-110">Child elements</span></span>

|<span data-ttu-id="7b5df-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b5df-111">**Element**</span></span>|<span data-ttu-id="7b5df-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b5df-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b5df-113">String</span><span class="sxs-lookup"><span data-stu-id="7b5df-113">String</span></span>](string.md) <br/> |<span data-ttu-id="7b5df-114">Contient une chaîne utilisée par des éléments, des contacts, des tâches et des conversations.</span><span class="sxs-lookup"><span data-stu-id="7b5df-114">Contains a string that is used by items, contacts, tasks, and conversations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7b5df-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b5df-115">Parent elements</span></span>

|<span data-ttu-id="7b5df-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b5df-116">**Element**</span></span>|<span data-ttu-id="7b5df-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b5df-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b5df-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="7b5df-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="7b5df-119">Contient l’État et le résultat d’une seule demande d' [opération FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7b5df-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7b5df-120">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="7b5df-120">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="7b5df-121">Contient la réponse pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7b5df-121">Contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b5df-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7b5df-122">Text value</span></span>

<span data-ttu-id="7b5df-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b5df-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7b5df-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b5df-124">Remarks</span></span>

<span data-ttu-id="7b5df-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b5df-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b5df-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b5df-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b5df-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b5df-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7b5df-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b5df-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7b5df-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7b5df-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7b5df-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7b5df-130">Validation File</span></span>  <br/> |<span data-ttu-id="7b5df-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7b5df-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7b5df-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b5df-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b5df-133">False</span><span class="sxs-lookup"><span data-stu-id="7b5df-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b5df-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b5df-134">See also</span></span>

- [<span data-ttu-id="7b5df-135">Opération FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7b5df-135">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="7b5df-136">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7b5df-136">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="7b5df-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7b5df-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

