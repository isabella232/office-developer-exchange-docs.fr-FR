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
description: L’élément MaxMessageSize représente la taille maximale des messages qu’un destinataire peut accepter.
ms.openlocfilehash: 727eed38a129800b7d38aa49c41cdacfa13e7a36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468410"
---
# <a name="maxmessagesize"></a><span data-ttu-id="8cb8b-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="8cb8b-103">MaxMessageSize</span></span>

<span data-ttu-id="8cb8b-104">L’élément **MaxMessageSize** représente la taille maximale des messages qu’un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="8cb8b-105">**int**</span><span class="sxs-lookup"><span data-stu-id="8cb8b-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8cb8b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8cb8b-106">Attributes and elements</span></span>

<span data-ttu-id="8cb8b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8cb8b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8cb8b-108">Attributes</span></span>

<span data-ttu-id="8cb8b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8cb8b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8cb8b-110">Child elements</span></span>

<span data-ttu-id="8cb8b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8cb8b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8cb8b-112">Parent elements</span></span>

|<span data-ttu-id="8cb8b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8cb8b-113">**Element**</span></span>|<span data-ttu-id="8cb8b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8cb8b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8cb8b-115">Infos-courrier</span><span class="sxs-lookup"><span data-stu-id="8cb8b-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="8cb8b-116">Représente les valeurs de différents types de conseils de courrier.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="8cb8b-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="8cb8b-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="8cb8b-118">Contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8cb8b-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8cb8b-119">Text value</span></span>

<span data-ttu-id="8cb8b-120">La valeur de texte est un entier qui représente la taille maximale des messages qu’un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="8cb8b-121">Cette valeur peut être mesurée en kilo-octets ou en mégaoctets.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8cb8b-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="8cb8b-122">Remarks</span></span>

<span data-ttu-id="8cb8b-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8cb8b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8cb8b-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8cb8b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8cb8b-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8cb8b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8cb8b-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8cb8b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8cb8b-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8cb8b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8cb8b-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8cb8b-128">Validation File</span></span>  <br/> |<span data-ttu-id="8cb8b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8cb8b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8cb8b-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8cb8b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8cb8b-131">False</span><span class="sxs-lookup"><span data-stu-id="8cb8b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8cb8b-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8cb8b-132">See also</span></span>



- [<span data-ttu-id="8cb8b-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8cb8b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

