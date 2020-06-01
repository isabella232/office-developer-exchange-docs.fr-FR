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
description: L’élément IncludeMimeContent spécifie si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément ou d’une pièce jointe est renvoyé dans la réponse.
ms.openlocfilehash: 6198e4bef2dc59e6e56a8d3cbe463dad13e544e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457192"
---
# <a name="includemimecontent"></a><span data-ttu-id="5c307-103">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="5c307-103">IncludeMimeContent</span></span>

<span data-ttu-id="5c307-104">L’élément **IncludeMimeContent** spécifie si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément ou d’une pièce jointe est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="5c307-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="5c307-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="5c307-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c307-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5c307-106">Attributes and elements</span></span>

<span data-ttu-id="5c307-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5c307-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c307-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5c307-108">Attributes</span></span>

<span data-ttu-id="5c307-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5c307-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c307-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5c307-110">Child elements</span></span>

<span data-ttu-id="5c307-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5c307-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c307-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5c307-112">Parent elements</span></span>

|<span data-ttu-id="5c307-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5c307-113">**Element**</span></span>|<span data-ttu-id="5c307-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c307-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c307-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="5c307-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="5c307-116">Identifie les propriétés supplémentaires à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="5c307-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="5c307-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="5c307-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="5c307-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5c307-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="5c307-119">Identifie les propriétés d’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="5c307-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="5c307-120">Voici les expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="5c307-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c307-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="5c307-121">Text value</span></span>

<span data-ttu-id="5c307-122">Cet élément peut avoir la **valeur true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="5c307-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="5c307-123">La valeur par défaut est **false**.</span><span class="sxs-lookup"><span data-stu-id="5c307-123">The default value is **false**.</span></span> <span data-ttu-id="5c307-124">Il s’agit d’un type de données booléen.</span><span class="sxs-lookup"><span data-stu-id="5c307-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c307-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="5c307-125">Remarks</span></span>

<span data-ttu-id="5c307-126">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="5c307-126">This element is optional.</span></span>
  
<span data-ttu-id="5c307-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5c307-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="5c307-128">Exemple</span><span class="sxs-lookup"><span data-stu-id="5c307-128">Example</span></span>

<span data-ttu-id="5c307-129">L’exemple de requête suivant illustre une procédure de définition de l’élément **IncludeMimeContent** .</span><span class="sxs-lookup"><span data-stu-id="5c307-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5c307-130">L’attribut ID de pièce jointe est tronqué pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5c307-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c307-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5c307-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c307-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5c307-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c307-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5c307-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5c307-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5c307-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c307-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5c307-135">Validation File</span></span>  <br/> |<span data-ttu-id="5c307-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c307-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c307-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5c307-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c307-138">False</span><span class="sxs-lookup"><span data-stu-id="5c307-138">False</span></span>  <br/> |
   

