---
title: UnsubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponse
api_type:
- schema
ms.assetid: 125e0326-6522-42cd-b20e-6977e6fde249
description: L’élément UnsubscribeResponse définit une réponse à une demande d’annulation d’abonnement.
ms.openlocfilehash: 1a8ddf93499acb7aa369ec9e91a7106e5cb4bd53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467199"
---
# <a name="unsubscriberesponse"></a><span data-ttu-id="17b96-103">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="17b96-103">UnsubscribeResponse</span></span>

<span data-ttu-id="17b96-104">L’élément **UnsubscribeResponse** définit une réponse à une demande d’annulation d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="17b96-104">The **UnsubscribeResponse** element defines a response to an Unsubscribe request.</span></span> 
  
```xml
<UnsubscribeResponse>
   <ResponseMessages/>
</UnsubscribeResponse>
```

 <span data-ttu-id="17b96-105">**UnsubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="17b96-105">**UnsubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17b96-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="17b96-106">Attributes and elements</span></span>

<span data-ttu-id="17b96-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="17b96-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17b96-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="17b96-108">Attributes</span></span>

<span data-ttu-id="17b96-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="17b96-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17b96-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="17b96-110">Child elements</span></span>

|<span data-ttu-id="17b96-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="17b96-111">**Element**</span></span>|<span data-ttu-id="17b96-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="17b96-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17b96-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="17b96-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="17b96-114">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="17b96-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17b96-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="17b96-115">Parent elements</span></span>

<span data-ttu-id="17b96-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="17b96-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17b96-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="17b96-117">Remarks</span></span>

<span data-ttu-id="17b96-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="17b96-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17b96-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="17b96-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17b96-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="17b96-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17b96-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="17b96-121">Schema name</span></span>  <br/> |<span data-ttu-id="17b96-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="17b96-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="17b96-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="17b96-123">Validation file</span></span>  <br/> |<span data-ttu-id="17b96-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="17b96-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17b96-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="17b96-125">Can be empty</span></span>  <br/> |<span data-ttu-id="17b96-126">False</span><span class="sxs-lookup"><span data-stu-id="17b96-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17b96-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="17b96-127">See also</span></span>



- [<span data-ttu-id="17b96-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="17b96-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

