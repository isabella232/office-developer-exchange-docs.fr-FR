---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: L’élément IncludeMimeContent Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément ou d’une pièce jointe est retourné dans la réponse.
ms.openlocfilehash: ddd6988be93231ac7c574a2e19c9ba4b562c7d0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827903"
---
# <a name="includemimecontent"></a><span data-ttu-id="e0d27-103">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="e0d27-103">IncludeMimeContent</span></span>

<span data-ttu-id="e0d27-104">L’élément **IncludeMimeContent** Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément ou d’une pièce jointe est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="e0d27-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="e0d27-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e0d27-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0d27-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e0d27-106">Attributes and elements</span></span>

<span data-ttu-id="e0d27-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e0d27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0d27-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e0d27-108">Attributes</span></span>

<span data-ttu-id="e0d27-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e0d27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0d27-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e0d27-110">Child elements</span></span>

<span data-ttu-id="e0d27-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e0d27-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0d27-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e0d27-112">Parent elements</span></span>

|<span data-ttu-id="e0d27-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e0d27-113">**Element**</span></span>|<span data-ttu-id="e0d27-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e0d27-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0d27-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="e0d27-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="e0d27-116">Identifie les propriétés supplémentaires pour retourner une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="e0d27-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="e0d27-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="e0d27-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="e0d27-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e0d27-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="e0d27-119">Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="e0d27-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="e0d27-120">Les expressions XPath pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="e0d27-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e0d27-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e0d27-121">Text value</span></span>

<span data-ttu-id="e0d27-122">Cet élément peut être **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="e0d27-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="e0d27-123">La valeur par défaut est **false**.</span><span class="sxs-lookup"><span data-stu-id="e0d27-123">The default value is **false**.</span></span> <span data-ttu-id="e0d27-124">Il s’agit d’un type de données Boolean.</span><span class="sxs-lookup"><span data-stu-id="e0d27-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e0d27-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="e0d27-125">Remarks</span></span>

<span data-ttu-id="e0d27-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="e0d27-126">This element is optional.</span></span>
  
<span data-ttu-id="e0d27-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e0d27-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e0d27-128">Exemple</span><span class="sxs-lookup"><span data-stu-id="e0d27-128">Example</span></span>

<span data-ttu-id="e0d27-129">Une demande de l’exemple suivant montre une procédure pour définir l’élément **IncludeMimeContent** .</span><span class="sxs-lookup"><span data-stu-id="e0d27-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e0d27-130">L’attribut Id de pièce jointe est tronqué afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e0d27-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0d27-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e0d27-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0d27-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e0d27-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0d27-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e0d27-133">Schema Name</span></span>  <br/> |<span data-ttu-id="e0d27-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e0d27-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0d27-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e0d27-135">Validation File</span></span>  <br/> |<span data-ttu-id="e0d27-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e0d27-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0d27-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e0d27-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0d27-138">False</span><span class="sxs-lookup"><span data-stu-id="e0d27-138">False</span></span>  <br/> |
   

