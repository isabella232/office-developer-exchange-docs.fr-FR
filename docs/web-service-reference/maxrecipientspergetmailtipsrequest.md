---
title: MaxRecipientsPerGetMailTipsRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: L’élément MaxRecipientsPerGetMailTipsRequest indique le nombre maximal de destinataires qui peuvent être transmis à l’opération GetMailTips.
ms.openlocfilehash: cec343182b364fce040d5e32928cbeb569a22124
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468403"
---
# <a name="maxrecipientspergetmailtipsrequest"></a><span data-ttu-id="4a726-103">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="4a726-103">MaxRecipientsPerGetMailTipsRequest</span></span>

<span data-ttu-id="4a726-104">L’élément **MaxRecipientsPerGetMailTipsRequest** indique le nombre maximal de destinataires qui peuvent être transmis à l' [opération GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4a726-104">The **MaxRecipientsPerGetMailTipsRequest** element indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 <span data-ttu-id="4a726-105">**int**</span><span class="sxs-lookup"><span data-stu-id="4a726-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a726-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a726-106">Attributes and elements</span></span>

<span data-ttu-id="4a726-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a726-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a726-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a726-108">Attributes</span></span>

<span data-ttu-id="4a726-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4a726-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a726-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a726-110">Child elements</span></span>

<span data-ttu-id="4a726-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4a726-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a726-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a726-112">Parent elements</span></span>

|<span data-ttu-id="4a726-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a726-113">**Element**</span></span>|<span data-ttu-id="4a726-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a726-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a726-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="4a726-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="4a726-116">Contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="4a726-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a726-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4a726-117">Text value</span></span>

<span data-ttu-id="4a726-118">La valeur de texte est un entier qui représente le nombre maximal de destinataires pouvant être transmis à l' [opération GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4a726-118">The text value is an integer that represents the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a726-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="4a726-119">Remarks</span></span>

<span data-ttu-id="4a726-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a726-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a726-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a726-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a726-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a726-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a726-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a726-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4a726-124">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4a726-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a726-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a726-125">Validation File</span></span>  <br/> |<span data-ttu-id="4a726-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a726-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a726-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a726-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a726-128">False</span><span class="sxs-lookup"><span data-stu-id="4a726-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a726-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a726-129">See also</span></span>



[<span data-ttu-id="4a726-130">Opération GetMailTips</span><span class="sxs-lookup"><span data-stu-id="4a726-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="4a726-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4a726-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

