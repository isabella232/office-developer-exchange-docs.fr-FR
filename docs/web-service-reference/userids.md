---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: L’élément UserIds contient un tableau d’utilisateurs délégués à récupérer ou à supprimer de la boîte aux lettres d’un principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: de4661226c154ef0d2d5ac55c57405e20c4d2aee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459776"
---
# <a name="userids"></a><span data-ttu-id="f1246-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="f1246-104">UserIds</span></span>

<span data-ttu-id="f1246-105">L’élément **userids** contient un tableau d’utilisateurs délégués à récupérer ou à supprimer de la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="f1246-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="f1246-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f1246-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="f1246-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="f1246-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1246-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1246-108">Attributes and elements</span></span>

<span data-ttu-id="f1246-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1246-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1246-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1246-110">Attributes</span></span>

<span data-ttu-id="f1246-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f1246-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1246-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1246-112">Child elements</span></span>

|<span data-ttu-id="f1246-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1246-113">**Element**</span></span>|<span data-ttu-id="f1246-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1246-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1246-115">UserId</span><span class="sxs-lookup"><span data-stu-id="f1246-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="f1246-116">Identifie un délégué à obtenir ou à supprimer de la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="f1246-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="f1246-117">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f1246-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1246-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1246-118">Parent elements</span></span>

|<span data-ttu-id="f1246-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1246-119">**Element**</span></span>|<span data-ttu-id="f1246-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1246-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1246-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="f1246-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="f1246-122">Définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1246-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="f1246-123">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f1246-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f1246-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="f1246-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="f1246-125">Définit une demande de suppression de délégués d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1246-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="f1246-126">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f1246-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1246-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1246-127">Remarks</span></span>

<span data-ttu-id="f1246-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f1246-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1246-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1246-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1246-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1246-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1246-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1246-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f1246-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f1246-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1246-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1246-133">Validation File</span></span>  <br/> |<span data-ttu-id="f1246-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1246-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1246-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1246-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1246-136">False</span><span class="sxs-lookup"><span data-stu-id="f1246-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1246-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1246-137">See also</span></span>



[<span data-ttu-id="f1246-138">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="f1246-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="f1246-139">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="f1246-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="f1246-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f1246-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

