---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: L’élément FolderShape identifie les propriétés de dossier à inclure dans une réponse GetFolder, FindFolder ou Opérationsyncfolderhierarchy.
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461344"
---
# <a name="foldershape"></a><span data-ttu-id="88a5b-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="88a5b-103">FolderShape</span></span>

<span data-ttu-id="88a5b-104">L’élément **FolderShape** identifie les propriétés de dossier à inclure dans une réponse [GetFolder](getfolder.md), [FindFolder](findfolder.md)ou [opérationsyncfolderhierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="88a5b-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="88a5b-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="88a5b-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88a5b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="88a5b-106">Attributes and elements</span></span>

<span data-ttu-id="88a5b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="88a5b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88a5b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="88a5b-108">Attributes</span></span>

<span data-ttu-id="88a5b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="88a5b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88a5b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="88a5b-110">Child elements</span></span>

|<span data-ttu-id="88a5b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="88a5b-111">**Element**</span></span>|<span data-ttu-id="88a5b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="88a5b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88a5b-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="88a5b-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="88a5b-114">Identifie la configuration de base des propriétés à renvoyer dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="88a5b-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="88a5b-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="88a5b-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="88a5b-116">Identifie les propriétés supplémentaires à renvoyer dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="88a5b-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88a5b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="88a5b-117">Parent elements</span></span>

|<span data-ttu-id="88a5b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="88a5b-118">**Element**</span></span>|<span data-ttu-id="88a5b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="88a5b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88a5b-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="88a5b-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="88a5b-121">Définit une demande pour identifier les dossiers d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="88a5b-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="88a5b-122">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="88a5b-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="88a5b-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="88a5b-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="88a5b-124">Définit une demande d’obtention d’un dossier à partir de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="88a5b-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="88a5b-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="88a5b-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="88a5b-126">Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="88a5b-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="88a5b-127">Définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.</span><span class="sxs-lookup"><span data-stu-id="88a5b-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="88a5b-128">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="88a5b-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88a5b-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="88a5b-129">Remarks</span></span>

<span data-ttu-id="88a5b-130">L’élément **FolderShape** est un élément enfant obligatoire de l’élément [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="88a5b-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="88a5b-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="88a5b-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="88a5b-132">Exemple</span><span class="sxs-lookup"><span data-stu-id="88a5b-132">Example</span></span>

<span data-ttu-id="88a5b-133">L’exemple de requête suivant montre comment rechercher tous les dossiers situés dans le premier niveau du dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="88a5b-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="88a5b-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="88a5b-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88a5b-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="88a5b-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="88a5b-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="88a5b-136">Schema Name</span></span>  <br/> |<span data-ttu-id="88a5b-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="88a5b-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="88a5b-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="88a5b-138">Validation File</span></span>  <br/> |<span data-ttu-id="88a5b-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="88a5b-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88a5b-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="88a5b-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="88a5b-141">False</span><span class="sxs-lookup"><span data-stu-id="88a5b-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88a5b-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="88a5b-142">See also</span></span>



[<span data-ttu-id="88a5b-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="88a5b-143">FindFolder</span></span>](findfolder.md)

