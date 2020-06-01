---
title: DiagnosticsLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DiagnosticsLevel
api_type:
- schema
ms.assetid: 66794226-f5e0-44f0-8a0e-1f194bb0ba0f
description: L’élément DiagnosticsLevel représente les informations de temps et de performances qui seront utilisées pour dériver le rapport.
ms.openlocfilehash: 3060d4f1b8449a5870d964bdfcdbf0d503905abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467829"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="55e9a-103">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="55e9a-103">DiagnosticsLevel</span></span>

<span data-ttu-id="55e9a-104">L’élément **DiagnosticsLevel** représente les informations de temps et de performances qui seront utilisées pour dériver le rapport.</span><span class="sxs-lookup"><span data-stu-id="55e9a-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="55e9a-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="55e9a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55e9a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="55e9a-106">Attributes and elements</span></span>

<span data-ttu-id="55e9a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="55e9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55e9a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="55e9a-108">Attributes</span></span>

<span data-ttu-id="55e9a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="55e9a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55e9a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="55e9a-110">Child elements</span></span>

<span data-ttu-id="55e9a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="55e9a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55e9a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="55e9a-112">Parent elements</span></span>

|<span data-ttu-id="55e9a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="55e9a-113">**Element**</span></span>|<span data-ttu-id="55e9a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="55e9a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55e9a-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="55e9a-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="55e9a-116">Contient des critères pour les types de messages à rechercher.</span><span class="sxs-lookup"><span data-stu-id="55e9a-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="55e9a-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="55e9a-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="55e9a-118">Contient la demande pour l' [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) afin de récupérer le rapport de suivi complet des messages pour l’ID spécifié.</span><span class="sxs-lookup"><span data-stu-id="55e9a-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55e9a-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="55e9a-119">Text value</span></span>

<span data-ttu-id="55e9a-120">Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="55e9a-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55e9a-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="55e9a-121">Remarks</span></span>

<span data-ttu-id="55e9a-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="55e9a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55e9a-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="55e9a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55e9a-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="55e9a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55e9a-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="55e9a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="55e9a-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="55e9a-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55e9a-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="55e9a-127">Validation File</span></span>  <br/> |<span data-ttu-id="55e9a-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="55e9a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55e9a-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="55e9a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="55e9a-130">False</span><span class="sxs-lookup"><span data-stu-id="55e9a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55e9a-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="55e9a-131">See also</span></span>

- [<span data-ttu-id="55e9a-132">Opération de GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="55e9a-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="55e9a-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="55e9a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

