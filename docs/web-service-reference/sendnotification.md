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
description: L’élément SendNotification contient les notifications de type transmission envoyées par l’ordinateur qui exécute Microsoft Exchange Server 2007 vers l’application cliente.
ms.openlocfilehash: 49f2f6cb7f5c8e1171b54ff965ee1d22accc9bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462114"
---
# <a name="sendnotification"></a><span data-ttu-id="d48a0-103">SendNotification</span><span class="sxs-lookup"><span data-stu-id="d48a0-103">SendNotification</span></span>

<span data-ttu-id="d48a0-104">L’élément **SendNotification** contient les notifications de type transmission envoyées par l’ordinateur qui exécute Microsoft Exchange Server 2007 vers l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="d48a0-104">The **SendNotification** element contains the push notifications that are sent by the computer that is running Microsoft Exchange Server 2007 to the client application.</span></span> 
  
```xml
<SendNotification>
   <ResponseMessages/>
</SendNotification>
```

 <span data-ttu-id="d48a0-105">**SendNotificationResponseType**</span><span class="sxs-lookup"><span data-stu-id="d48a0-105">**SendNotificationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d48a0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d48a0-106">Attributes and elements</span></span>

<span data-ttu-id="d48a0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d48a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d48a0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d48a0-108">Attributes</span></span>

<span data-ttu-id="d48a0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d48a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d48a0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d48a0-110">Child elements</span></span>

|<span data-ttu-id="d48a0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d48a0-111">**Element**</span></span>|<span data-ttu-id="d48a0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d48a0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d48a0-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d48a0-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d48a0-114">Contient les notifications de type transmission envoyées par le serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="d48a0-114">Contains the push notifications that are sent by the Client Access server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d48a0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d48a0-115">Parent elements</span></span>

<span data-ttu-id="d48a0-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d48a0-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d48a0-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="d48a0-117">Remarks</span></span>

<span data-ttu-id="d48a0-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d48a0-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d48a0-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d48a0-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d48a0-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d48a0-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d48a0-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d48a0-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d48a0-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d48a0-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d48a0-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d48a0-123">Validation File</span></span>  <br/> |<span data-ttu-id="d48a0-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d48a0-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d48a0-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d48a0-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d48a0-126">False</span><span class="sxs-lookup"><span data-stu-id="d48a0-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d48a0-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d48a0-127">See also</span></span>



- [<span data-ttu-id="d48a0-128">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d48a0-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d48a0-129">Notifications d’événements dans EWS</span><span class="sxs-lookup"><span data-stu-id="d48a0-129">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
  
[<span data-ttu-id="d48a0-130">Exemple d'application de notification Push</span><span class="sxs-lookup"><span data-stu-id="d48a0-130">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

