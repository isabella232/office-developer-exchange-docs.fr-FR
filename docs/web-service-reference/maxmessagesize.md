---
title: MaxMessageSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxMessageSize
api_type:
- schema
ms.assetid: bb98ac72-9409-4332-81bb-ee3bebb9a00e
description: L’élément MaxMessageSize représente la taille maximale des messages qu'un destinataire peut accepter.
ms.openlocfilehash: 13a5679a03420655356269a7e8b5e22950724164
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828383"
---
# <a name="maxmessagesize"></a><span data-ttu-id="d0887-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="d0887-103">MaxMessageSize</span></span>

<span data-ttu-id="d0887-104">L’élément **MaxMessageSize** représente la taille maximale des messages qu'un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="d0887-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="d0887-105">**int**</span><span class="sxs-lookup"><span data-stu-id="d0887-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0887-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d0887-106">Attributes and elements</span></span>

<span data-ttu-id="d0887-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d0887-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0887-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d0887-108">Attributes</span></span>

<span data-ttu-id="d0887-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d0887-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0887-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d0887-110">Child elements</span></span>

<span data-ttu-id="d0887-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d0887-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0887-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d0887-112">Parent elements</span></span>

|<span data-ttu-id="d0887-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0887-113">**Element**</span></span>|<span data-ttu-id="d0887-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0887-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0887-115">Les infos-courrier</span><span class="sxs-lookup"><span data-stu-id="d0887-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="d0887-116">Représente les valeurs pour les différents types d’astuces de la messagerie.</span><span class="sxs-lookup"><span data-stu-id="d0887-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="d0887-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="d0887-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="d0887-118">Contient des informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="d0887-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0887-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d0887-119">Text value</span></span>

<span data-ttu-id="d0887-120">La valeur de texte est un entier qui représente la taille maximale des messages d’un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="d0887-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="d0887-121">Cette valeur peut être exprimée en kilo-octets ou en mégaoctets.</span><span class="sxs-lookup"><span data-stu-id="d0887-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0887-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="d0887-122">Remarks</span></span>

<span data-ttu-id="d0887-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0887-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0887-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d0887-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0887-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d0887-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0887-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d0887-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d0887-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d0887-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0887-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d0887-128">Validation File</span></span>  <br/> |<span data-ttu-id="d0887-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0887-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0887-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d0887-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0887-131">False</span><span class="sxs-lookup"><span data-stu-id="d0887-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0887-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d0887-132">See also</span></span>



- [<span data-ttu-id="d0887-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d0887-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

