---
title: UnpinTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1034b013-ef34-4e72-99b3-38bff475b3e8
description: L’élément UnpinTeamMailbox contient la demande de désépinglage d’une boîte aux lettres de site du client en la supprimant de la réponse de découverte automatique.
ms.openlocfilehash: a6b01bfa9c5908765ff04ef7f5edbef0b99a9be2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467241"
---
# <a name="unpinteammailbox"></a><span data-ttu-id="f08ef-103">UnpinTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="f08ef-103">UnpinTeamMailbox</span></span>

<span data-ttu-id="f08ef-104">L’élément **UnpinTeamMailbox** contient la demande de désépinglage d’une boîte aux lettres de site du client en la supprimant de la réponse de **découverte automatique** .</span><span class="sxs-lookup"><span data-stu-id="f08ef-104">The **UnpinTeamMailbox** element contains the request to unpin a site mailbox from the client by removing it from the **Autodiscover** response.</span></span> 
  
```XML
<UnpinTeamMailbox>
   <EmailAddress/>
</UnpinTeamMailbox>
```

 <span data-ttu-id="f08ef-105">**UnpinTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="f08ef-105">**UnpinTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f08ef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f08ef-106">Attributes and elements</span></span>

<span data-ttu-id="f08ef-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f08ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f08ef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f08ef-108">Attributes</span></span>

<span data-ttu-id="f08ef-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f08ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f08ef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f08ef-110">Child elements</span></span>

[<span data-ttu-id="f08ef-111">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f08ef-111">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
  
### <a name="parent-elements"></a><span data-ttu-id="f08ef-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f08ef-112">Parent elements</span></span>

<span data-ttu-id="f08ef-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f08ef-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f08ef-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="f08ef-114">Remarks</span></span>

<span data-ttu-id="f08ef-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f08ef-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f08ef-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f08ef-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f08ef-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f08ef-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f08ef-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f08ef-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f08ef-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f08ef-119">Schema name</span></span>  <br/> |<span data-ttu-id="f08ef-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f08ef-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f08ef-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f08ef-121">Validation file</span></span>  <br/> |<span data-ttu-id="f08ef-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f08ef-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f08ef-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f08ef-123">Can be empty</span></span>  <br/> ||
   

