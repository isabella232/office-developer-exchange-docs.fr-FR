---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: L’élément GetDelegate définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756571"
---
# <a name="getdelegate"></a><span data-ttu-id="54c7e-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="54c7e-104">GetDelegate</span></span>

<span data-ttu-id="54c7e-105">L’élément **GetDelegate** définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="54c7e-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="54c7e-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="54c7e-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="54c7e-107">**GetDelegateType**</span><span class="sxs-lookup"><span data-stu-id="54c7e-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54c7e-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54c7e-108">Attributes and elements</span></span>

<span data-ttu-id="54c7e-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54c7e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54c7e-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="54c7e-110">Attributes</span></span>

|<span data-ttu-id="54c7e-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="54c7e-111">**Attribute**</span></span>|<span data-ttu-id="54c7e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="54c7e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54c7e-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="54c7e-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="54c7e-114">Indique si la réponse contient les paramètres d’autorisation pour chaque utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="54c7e-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="54c7e-115">Valeurs des attributs IncludePermissions</span><span class="sxs-lookup"><span data-stu-id="54c7e-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="54c7e-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="54c7e-116">**Value**</span></span>|<span data-ttu-id="54c7e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="54c7e-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="54c7e-118">**True**</span><span class="sxs-lookup"><span data-stu-id="54c7e-118">**True**</span></span> <br/> |<span data-ttu-id="54c7e-119">Déléguer l’utilisateur en plus des informations utilisateur délégué retourné dans l’élément [UserId](userid.md) les autorisations sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="54c7e-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="54c7e-120">**False**</span><span class="sxs-lookup"><span data-stu-id="54c7e-120">**False**</span></span> <br/> |<span data-ttu-id="54c7e-121">Informations [UserId](userid.md) sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="54c7e-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="54c7e-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54c7e-122">Child elements</span></span>

|<span data-ttu-id="54c7e-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54c7e-123">**Element**</span></span>|<span data-ttu-id="54c7e-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="54c7e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54c7e-125">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="54c7e-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="54c7e-126">Identifie la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="54c7e-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="54c7e-127">ID utilisateur</span><span class="sxs-lookup"><span data-stu-id="54c7e-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="54c7e-128">Contient un tableau d’utilisateurs délégué à obtenir à partir de la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="54c7e-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="54c7e-129">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="54c7e-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54c7e-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54c7e-130">Parent elements</span></span>

<span data-ttu-id="54c7e-131">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54c7e-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54c7e-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="54c7e-132">Remarks</span></span>

<span data-ttu-id="54c7e-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="54c7e-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54c7e-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="54c7e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54c7e-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="54c7e-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54c7e-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="54c7e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="54c7e-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="54c7e-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54c7e-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="54c7e-138">Validation File</span></span>  <br/> |<span data-ttu-id="54c7e-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54c7e-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54c7e-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="54c7e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="54c7e-141">False</span><span class="sxs-lookup"><span data-stu-id="54c7e-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54c7e-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54c7e-142">See also</span></span>



[<span data-ttu-id="54c7e-143">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="54c7e-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="54c7e-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="54c7e-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

