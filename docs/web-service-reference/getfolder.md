---
title: GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 34e4c9ea-adcd-46bd-ae8f-7abb256c585a
description: L’élément GetFolder définit une demande pour obtenir un dossier à partir d’une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: 233da6ce57683350d4a13f6585593ac09438f0e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756623"
---
# <a name="getfolder"></a><span data-ttu-id="4ac31-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="4ac31-103">GetFolder</span></span>

<span data-ttu-id="4ac31-104">L’élément **GetFolder** définit une demande pour obtenir un dossier à partir d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ac31-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="4ac31-105">**GetFolderType**</span><span class="sxs-lookup"><span data-stu-id="4ac31-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ac31-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4ac31-106">Attributes and elements</span></span>

<span data-ttu-id="4ac31-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4ac31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ac31-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4ac31-108">Attributes</span></span>

<span data-ttu-id="4ac31-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4ac31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ac31-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4ac31-110">Child elements</span></span>

|<span data-ttu-id="4ac31-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4ac31-111">**Element**</span></span>|<span data-ttu-id="4ac31-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4ac31-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ac31-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="4ac31-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="4ac31-114">Identifie les propriétés à obtenir pour chaque dossier identifié dans l’élément [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="4ac31-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="4ac31-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="4ac31-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="4ac31-116">Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à obtenir à partir d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ac31-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ac31-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4ac31-117">Parent elements</span></span>

<span data-ttu-id="4ac31-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4ac31-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ac31-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="4ac31-119">Remarks</span></span>

<span data-ttu-id="4ac31-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4ac31-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ac31-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4ac31-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ac31-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4ac31-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4ac31-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4ac31-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4ac31-124">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="4ac31-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="4ac31-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4ac31-125">Validation File</span></span>  <br/> |<span data-ttu-id="4ac31-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4ac31-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4ac31-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4ac31-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ac31-128">False</span><span class="sxs-lookup"><span data-stu-id="4ac31-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ac31-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4ac31-129">See also</span></span>



[<span data-ttu-id="4ac31-130">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="4ac31-130">GetFolder operation</span></span>](getfolder-operation.md)

