---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: L’élément FilterHtmlContent Spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’un élément ou d’une pièce jointe.
ms.openlocfilehash: db181eff9586061d728a5e4ef55a78f4955b5713
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756369"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="45c5b-103">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="45c5b-103">FilterHtmlContent</span></span>

<span data-ttu-id="45c5b-104">L’élément **FilterHtmlContent** Spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’un élément ou d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="45c5b-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="45c5b-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="45c5b-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45c5b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="45c5b-106">Attributes and elements</span></span>

<span data-ttu-id="45c5b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="45c5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45c5b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="45c5b-108">Attributes</span></span>

<span data-ttu-id="45c5b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="45c5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45c5b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="45c5b-110">Child elements</span></span>

<span data-ttu-id="45c5b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="45c5b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="45c5b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="45c5b-112">Parent elements</span></span>

|<span data-ttu-id="45c5b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="45c5b-113">**Element**</span></span>|<span data-ttu-id="45c5b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="45c5b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45c5b-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="45c5b-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="45c5b-116">Identifie les propriétés supplémentaires pour retourner une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="45c5b-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="45c5b-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="45c5b-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="45c5b-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="45c5b-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="45c5b-119">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="45c5b-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="45c5b-120">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="45c5b-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="45c5b-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="45c5b-121">Text value</span></span>

<span data-ttu-id="45c5b-122">Cet élément peut être **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="45c5b-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="45c5b-123">La valeur par défaut est **false**.</span><span class="sxs-lookup"><span data-stu-id="45c5b-123">The default value is **false**.</span></span> <span data-ttu-id="45c5b-124">Il s’agit d’un type de données Boolean.</span><span class="sxs-lookup"><span data-stu-id="45c5b-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45c5b-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="45c5b-125">Remarks</span></span>

<span data-ttu-id="45c5b-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="45c5b-126">This element is optional.</span></span>
  
<span data-ttu-id="45c5b-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="45c5b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45c5b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="45c5b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45c5b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="45c5b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="45c5b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="45c5b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="45c5b-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="45c5b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="45c5b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="45c5b-132">Validation File</span></span>  <br/> |<span data-ttu-id="45c5b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="45c5b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="45c5b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="45c5b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="45c5b-135">False</span><span class="sxs-lookup"><span data-stu-id="45c5b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45c5b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="45c5b-136">See also</span></span>

- [<span data-ttu-id="45c5b-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45c5b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

