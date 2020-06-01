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
description: L’élément GetFolder définit une demande pour obtenir un dossier à partir d’une boîte aux lettres dans la Banque d’Exchange.
ms.openlocfilehash: 41d2b1ab5fcd5d2d60c399e8070ca957ee4b66e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458704"
---
# <a name="getfolder"></a><span data-ttu-id="a4010-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="a4010-103">GetFolder</span></span>

<span data-ttu-id="a4010-104">L’élément **GetFolder** définit une demande pour obtenir un dossier à partir d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4010-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="a4010-105">**GetFolderType**</span><span class="sxs-lookup"><span data-stu-id="a4010-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4010-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a4010-106">Attributes and elements</span></span>

<span data-ttu-id="a4010-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a4010-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4010-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a4010-108">Attributes</span></span>

<span data-ttu-id="a4010-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a4010-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4010-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a4010-110">Child elements</span></span>

|<span data-ttu-id="a4010-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a4010-111">**Element**</span></span>|<span data-ttu-id="a4010-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="a4010-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4010-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="a4010-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="a4010-114">Identifie les propriétés à obtenir pour chaque dossier identifié dans l’élément [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="a4010-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="a4010-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="a4010-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="a4010-116">Contient un tableau des identificateurs de dossier utilisés pour identifier les dossiers à obtenir à partir d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4010-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4010-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a4010-117">Parent elements</span></span>

<span data-ttu-id="a4010-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a4010-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a4010-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="a4010-119">Remarks</span></span>

<span data-ttu-id="a4010-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a4010-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4010-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a4010-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4010-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a4010-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4010-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a4010-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a4010-124">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="a4010-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="a4010-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a4010-125">Validation File</span></span>  <br/> |<span data-ttu-id="a4010-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a4010-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4010-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a4010-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4010-128">False</span><span class="sxs-lookup"><span data-stu-id="a4010-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4010-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a4010-129">See also</span></span>



[<span data-ttu-id="a4010-130">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="a4010-130">GetFolder operation</span></span>](getfolder-operation.md)

