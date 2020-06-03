---
title: Notifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: L’élément notifications contient un tableau d’informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.
ms.openlocfilehash: 88fc56ba6e672e3dea7a1d31f7cc1fda018b9a15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462618"
---
# <a name="notifications"></a><span data-ttu-id="00100-103">Notifications</span><span class="sxs-lookup"><span data-stu-id="00100-103">Notifications</span></span>

<span data-ttu-id="00100-104">L’élément **notifications** contient un tableau d’informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="00100-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="00100-105">**NonEmptyArrayOfNotificationsType**</span><span class="sxs-lookup"><span data-stu-id="00100-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00100-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00100-106">Attributes and elements</span></span>

<span data-ttu-id="00100-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00100-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00100-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00100-108">Attributes</span></span>

<span data-ttu-id="00100-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00100-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00100-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00100-110">Child elements</span></span>

|<span data-ttu-id="00100-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00100-111">**Element**</span></span>|<span data-ttu-id="00100-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="00100-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00100-113">Notification</span><span class="sxs-lookup"><span data-stu-id="00100-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="00100-114">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="00100-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00100-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00100-115">Parent elements</span></span>

|<span data-ttu-id="00100-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00100-116">**Element**</span></span>|<span data-ttu-id="00100-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="00100-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00100-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00100-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="00100-119">Contient l’État et le résultat d’une seule demande d' [opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="00100-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00100-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="00100-120">Text value</span></span>

<span data-ttu-id="00100-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00100-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00100-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="00100-122">Remarks</span></span>

<span data-ttu-id="00100-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="00100-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00100-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00100-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00100-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00100-125">Namespace</span></span>  <br/> |<span data-ttu-id="00100-126">https://schemas.microsoft.com/exchange/services/2006/messages et https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="00100-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="00100-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00100-127">Schema Name</span></span>  <br/> |<span data-ttu-id="00100-128">Schéma des messages ; Schéma de types</span><span class="sxs-lookup"><span data-stu-id="00100-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="00100-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00100-129">Validation File</span></span>  <br/> |<span data-ttu-id="00100-130">Messages. xsd ; Types. xsd</span><span class="sxs-lookup"><span data-stu-id="00100-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00100-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00100-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="00100-132">False</span><span class="sxs-lookup"><span data-stu-id="00100-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00100-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00100-133">See also</span></span>



[<span data-ttu-id="00100-134">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="00100-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="00100-135">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="00100-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="00100-136">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="00100-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="00100-137">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="00100-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="00100-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="00100-138">Subscribe operation</span></span>](subscribe-operation.md)

