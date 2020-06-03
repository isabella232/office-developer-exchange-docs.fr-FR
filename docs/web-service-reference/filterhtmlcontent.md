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
description: L’élément FilterHtmlContent spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’un élément ou d’une pièce jointe.
ms.openlocfilehash: 28e3be86b550c3f330fbb6846b64732b5674304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462674"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="85cd8-103">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="85cd8-103">FilterHtmlContent</span></span>

<span data-ttu-id="85cd8-104">L’élément **FilterHtmlContent** spécifie si le contenu HTML potentiellement dangereux est filtré à partir d’un élément ou d’une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="85cd8-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="85cd8-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="85cd8-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85cd8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85cd8-106">Attributes and elements</span></span>

<span data-ttu-id="85cd8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85cd8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85cd8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="85cd8-108">Attributes</span></span>

<span data-ttu-id="85cd8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="85cd8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85cd8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85cd8-110">Child elements</span></span>

<span data-ttu-id="85cd8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="85cd8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85cd8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85cd8-112">Parent elements</span></span>

|<span data-ttu-id="85cd8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85cd8-113">**Element**</span></span>|<span data-ttu-id="85cd8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="85cd8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85cd8-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="85cd8-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="85cd8-116">Identifie les propriétés supplémentaires à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="85cd8-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="85cd8-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="85cd8-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="85cd8-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="85cd8-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="85cd8-119">Identifie les propriétés d’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="85cd8-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="85cd8-120">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="85cd8-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85cd8-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="85cd8-121">Text value</span></span>

<span data-ttu-id="85cd8-122">Cet élément peut avoir la **valeur true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="85cd8-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="85cd8-123">La valeur par défaut est **false**.</span><span class="sxs-lookup"><span data-stu-id="85cd8-123">The default value is **false**.</span></span> <span data-ttu-id="85cd8-124">Il s’agit d’un type de données booléen.</span><span class="sxs-lookup"><span data-stu-id="85cd8-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85cd8-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="85cd8-125">Remarks</span></span>

<span data-ttu-id="85cd8-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="85cd8-126">This element is optional.</span></span>
  
<span data-ttu-id="85cd8-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server et sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="85cd8-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85cd8-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85cd8-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85cd8-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85cd8-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85cd8-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85cd8-130">Schema Name</span></span>  <br/> |<span data-ttu-id="85cd8-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="85cd8-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="85cd8-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85cd8-132">Validation File</span></span>  <br/> |<span data-ttu-id="85cd8-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85cd8-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85cd8-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85cd8-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="85cd8-135">False</span><span class="sxs-lookup"><span data-stu-id="85cd8-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85cd8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85cd8-136">See also</span></span>

- [<span data-ttu-id="85cd8-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85cd8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

