---
title: CopyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponse
api_type:
- schema
ms.assetid: 5bfbb4d3-e2ed-4b84-96f7-2175f1947aed
description: L’élément CopyFolderResponse définit une réponse à une demande CopyFolder.
ms.openlocfilehash: aaf5d2bde8c9ba6b0c8aa6345af39dd9a6006ae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458515"
---
# <a name="copyfolderresponse"></a><span data-ttu-id="fc493-103">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="fc493-103">CopyFolderResponse</span></span>

<span data-ttu-id="fc493-104">L’élément **CopyFolderResponse** définit une réponse à une demande CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="fc493-104">The **CopyFolderResponse** element defines a response to a CopyFolder request.</span></span> 
  
```xml
<CopyFolderResponse>
   <ResponseMessages/>
</CopyFolderResponse>
```

 <span data-ttu-id="fc493-105">**CopyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="fc493-105">**CopyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc493-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fc493-106">Attributes and elements</span></span>

<span data-ttu-id="fc493-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fc493-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc493-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fc493-108">Attributes</span></span>

<span data-ttu-id="fc493-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fc493-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc493-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fc493-110">Child elements</span></span>

|<span data-ttu-id="fc493-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc493-111">**Element**</span></span>|<span data-ttu-id="fc493-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc493-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc493-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fc493-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fc493-114">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc493-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc493-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fc493-115">Parent elements</span></span>

<span data-ttu-id="fc493-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fc493-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc493-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="fc493-117">Remarks</span></span>

<span data-ttu-id="fc493-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fc493-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc493-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fc493-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc493-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fc493-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc493-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fc493-121">Schema name</span></span>  <br/> |<span data-ttu-id="fc493-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fc493-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc493-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fc493-123">Validation file</span></span>  <br/> |<span data-ttu-id="fc493-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fc493-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc493-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fc493-125">Can be empty</span></span>  <br/> |<span data-ttu-id="fc493-126">False</span><span class="sxs-lookup"><span data-stu-id="fc493-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc493-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fc493-127">See also</span></span>



[<span data-ttu-id="fc493-128">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="fc493-128">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="fc493-129">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="fc493-129">CopyFolder</span></span>](copyfolder.md)


- [<span data-ttu-id="fc493-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fc493-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

