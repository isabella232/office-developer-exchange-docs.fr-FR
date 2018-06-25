---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: L’élément ParentItemId identifie l’élément parent qui lie à une pièce jointe associée.
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828703"
---
# <a name="parentitemid"></a><span data-ttu-id="8e91b-103">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="8e91b-103">ParentItemId</span></span>

<span data-ttu-id="8e91b-104">L’élément **ParentItemId** identifie l’élément parent qui lie à une pièce jointe associée.</span><span class="sxs-lookup"><span data-stu-id="8e91b-104">The **ParentItemId** element identifies the parent item that links to an associated attachment.</span></span> 
  
- [<span data-ttu-id="8e91b-105">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="8e91b-105">CreateAttachment</span></span>](createattachment.md)
  
- [<span data-ttu-id="8e91b-106">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="8e91b-106">ParentItemId</span></span>](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

<span data-ttu-id="8e91b-107">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="8e91b-107">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8e91b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8e91b-108">Attributes and elements</span></span>

<span data-ttu-id="8e91b-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8e91b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e91b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="8e91b-110">Attributes</span></span>

|<span data-ttu-id="8e91b-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="8e91b-111">**Attribute**</span></span>|<span data-ttu-id="8e91b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8e91b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e91b-113">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="8e91b-113">**Id**</span></span> <br/> |<span data-ttu-id="8e91b-114">Identifie un seul élément dans la banque d’informations Exchange à associer à une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8e91b-114">Identifies a single item in the Exchange store to associate with an attachment.</span></span> <span data-ttu-id="8e91b-115">Cette valeur est une chaîne.</span><span class="sxs-lookup"><span data-stu-id="8e91b-115">This value is a string.</span></span> <span data-ttu-id="8e91b-116">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="8e91b-116">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="8e91b-117">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="8e91b-117">**ChangeKey**</span></span> <br/> |<span data-ttu-id="8e91b-118">Identifie une version non spécifiée d’un élément identifié par l’attribut **Id** de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e91b-118">Identifies an unspecified version of an item that is identified by the **Id** attribute in the Exchange store.</span></span> <span data-ttu-id="8e91b-119">Cela permet de vous assurer qu’un élément en cours est utilisé lorsqu’il est mis à jour avec une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="8e91b-119">This is used to make sure that a current item is used when it is updated with an attachment.</span></span> <span data-ttu-id="8e91b-120">Cette valeur est une chaîne.</span><span class="sxs-lookup"><span data-stu-id="8e91b-120">This value is a string.</span></span> <span data-ttu-id="8e91b-121">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="8e91b-121">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8e91b-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8e91b-122">Child elements</span></span>

<span data-ttu-id="8e91b-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8e91b-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e91b-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8e91b-124">Parent elements</span></span>

|<span data-ttu-id="8e91b-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8e91b-125">**Element**</span></span>|<span data-ttu-id="8e91b-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="8e91b-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e91b-127">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="8e91b-127">CreateAttachment</span></span>](createattachment.md) <br/> |<span data-ttu-id="8e91b-128">Définit une demande pour créer une pièce jointe à un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8e91b-128">Defines a request to create an attachment to an item in a mailbox.</span></span>  <br/> <span data-ttu-id="8e91b-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8e91b-129">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8e91b-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="8e91b-130">Remarks</span></span>

<span data-ttu-id="8e91b-131">Cet élément est requis dans l' [opération CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="8e91b-131">This element is required in the [CreateAttachment operation](createattachment-operation.md).</span></span> <span data-ttu-id="8e91b-132">Cet élément est identique à l’élément [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="8e91b-132">This element is basically the same as the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="8e91b-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8e91b-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e91b-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8e91b-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e91b-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8e91b-135">Namespace</span></span>  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|<span data-ttu-id="8e91b-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8e91b-136">Schema Name</span></span>  <br/> |<span data-ttu-id="8e91b-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8e91b-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8e91b-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8e91b-138">Validation File</span></span>  <br/> |<span data-ttu-id="8e91b-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8e91b-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8e91b-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8e91b-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e91b-141">False</span><span class="sxs-lookup"><span data-stu-id="8e91b-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e91b-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8e91b-142">See also</span></span>

- [<span data-ttu-id="8e91b-143">Opération CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="8e91b-143">CreateAttachment operation</span></span>](createattachment-operation.md)

