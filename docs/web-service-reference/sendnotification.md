---
title: SendNotification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotification
api_type:
- schema
ms.assetid: e45c4451-a286-4aec-a691-119ec41c58e0
description: L’élément SendNotification contient les notifications push envoyées par l’ordinateur qui exécute Microsoft Exchange Server 2007 à l’application cliente.
ms.openlocfilehash: 2288dbb5cf97b57a64b3c645eb72836342f4c178
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829345"
---
# <a name="sendnotification"></a><span data-ttu-id="222f1-103">SendNotification</span><span class="sxs-lookup"><span data-stu-id="222f1-103">SendNotification</span></span>

<span data-ttu-id="222f1-104">L’élément **SendNotification** contient les notifications push envoyées par l’ordinateur qui exécute Microsoft Exchange Server 2007 à l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="222f1-104">The **SendNotification** element contains the push notifications that are sent by the computer that is running Microsoft Exchange Server 2007 to the client application.</span></span> 
  
```xml
<SendNotification>
   <ResponseMessages/>
</SendNotification>
```

 <span data-ttu-id="222f1-105">**SendNotificationResponseType**</span><span class="sxs-lookup"><span data-stu-id="222f1-105">**SendNotificationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="222f1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="222f1-106">Attributes and elements</span></span>

<span data-ttu-id="222f1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="222f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="222f1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="222f1-108">Attributes</span></span>

<span data-ttu-id="222f1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="222f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="222f1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="222f1-110">Child elements</span></span>

|<span data-ttu-id="222f1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="222f1-111">**Element**</span></span>|<span data-ttu-id="222f1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="222f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="222f1-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="222f1-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="222f1-114">Contient les notifications push envoyées par le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="222f1-114">Contains the push notifications that are sent by the Client Access server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="222f1-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="222f1-115">Parent elements</span></span>

<span data-ttu-id="222f1-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="222f1-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="222f1-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="222f1-117">Remarks</span></span>

<span data-ttu-id="222f1-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="222f1-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="222f1-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="222f1-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="222f1-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="222f1-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="222f1-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="222f1-121">Schema Name</span></span>  <br/> |<span data-ttu-id="222f1-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="222f1-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="222f1-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="222f1-123">Validation File</span></span>  <br/> |<span data-ttu-id="222f1-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="222f1-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="222f1-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="222f1-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="222f1-126">False</span><span class="sxs-lookup"><span data-stu-id="222f1-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="222f1-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="222f1-127">See also</span></span>



- [<span data-ttu-id="222f1-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="222f1-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="222f1-129">Notifications d’événement dans EWS</span><span class="sxs-lookup"><span data-stu-id="222f1-129">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
  
[<span data-ttu-id="222f1-130">Exemple d'application de notification Push</span><span class="sxs-lookup"><span data-stu-id="222f1-130">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

