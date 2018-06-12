---
title: ViewPrivateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: L’élément ViewPrivateItems indique si une délégué utilisateur ou l’application cliente a l’autorisation d’afficher des éléments privées dans la boîte aux lettres de l’entité de sécurité.
ms.openlocfilehash: c35f24ae79e907424cb5cfb0efeec2307334ca12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839018"
---
# <a name="viewprivateitems"></a><span data-ttu-id="bacfa-103">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="bacfa-103">ViewPrivateItems</span></span>

<span data-ttu-id="bacfa-104">L’élément **ViewPrivateItems** indique si une délégué utilisateur ou l’application cliente a l’autorisation d’afficher des éléments privées dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="bacfa-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="bacfa-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bacfa-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bacfa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bacfa-106">Attributes and elements</span></span>

<span data-ttu-id="bacfa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bacfa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bacfa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bacfa-108">Attributes</span></span>

<span data-ttu-id="bacfa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bacfa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bacfa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bacfa-110">Child elements</span></span>

<span data-ttu-id="bacfa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bacfa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bacfa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bacfa-112">Parent elements</span></span>

|<span data-ttu-id="bacfa-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bacfa-113">**Element**</span></span>|<span data-ttu-id="bacfa-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bacfa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bacfa-115">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="bacfa-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="bacfa-116">Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="bacfa-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="bacfa-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="bacfa-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="bacfa-p101">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="bacfa-p101">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bacfa-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bacfa-120">Text value</span></span>

<span data-ttu-id="bacfa-121">La valeur **true** indique que le client ou un délégué peut afficher les éléments privées dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="bacfa-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="bacfa-122">La valeur **false** indique que les éléments privés ne sont pas visibles pour un client ou un délégué.</span><span class="sxs-lookup"><span data-stu-id="bacfa-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bacfa-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="bacfa-123">Remarks</span></span>

<span data-ttu-id="bacfa-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bacfa-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bacfa-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bacfa-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bacfa-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bacfa-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bacfa-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bacfa-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bacfa-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bacfa-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="bacfa-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bacfa-129">Validation File</span></span>  <br/> |<span data-ttu-id="bacfa-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bacfa-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bacfa-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bacfa-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="bacfa-132">False</span><span class="sxs-lookup"><span data-stu-id="bacfa-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bacfa-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bacfa-133">See also</span></span>



[<span data-ttu-id="bacfa-134">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="bacfa-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="bacfa-135">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="bacfa-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="bacfa-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bacfa-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="bacfa-137">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="bacfa-137">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

