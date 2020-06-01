---
title: Application
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: L’élément App contient des informations sur un fichier manifeste XML pour une application de messagerie installée dans une boîte aux lettres.
ms.openlocfilehash: b5870164b059d2e50930ee33c09cbd030501f171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460357"
---
# <a name="app"></a><span data-ttu-id="2ca54-103">Application</span><span class="sxs-lookup"><span data-stu-id="2ca54-103">App</span></span>

<span data-ttu-id="2ca54-104">L’élément **app** contient des informations sur un fichier manifeste XML pour une application de messagerie installée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2ca54-104">The **App** element contains information about an XML manifest file for a mail app that is installed in a mailbox.</span></span> 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2ca54-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2ca54-105">Attributes and elements</span></span>

<span data-ttu-id="2ca54-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2ca54-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ca54-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="2ca54-107">Attributes</span></span>

<span data-ttu-id="2ca54-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2ca54-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ca54-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2ca54-109">Child elements</span></span>

<span data-ttu-id="2ca54-110">[Métadonnées](metadata-ex15websvcsotherref.md)  |  [Manifeste](manifest.md)</span><span class="sxs-lookup"><span data-stu-id="2ca54-110">[Metadata](metadata-ex15websvcsotherref.md) | [Manifest](manifest.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ca54-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2ca54-111">Parent elements</span></span>

[<span data-ttu-id="2ca54-112">Applications</span><span class="sxs-lookup"><span data-stu-id="2ca54-112">Apps</span></span>](apps.md)
  
## <a name="remarks"></a><span data-ttu-id="2ca54-113">Remarques</span><span class="sxs-lookup"><span data-stu-id="2ca54-113">Remarks</span></span>

<span data-ttu-id="2ca54-114">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2ca54-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="2ca54-115">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ca54-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ca54-116">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2ca54-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ca54-117">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2ca54-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ca54-118">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2ca54-118">Schema Name</span></span>  <br/> |<span data-ttu-id="2ca54-119">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2ca54-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ca54-120">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2ca54-120">Validation File</span></span>  <br/> |<span data-ttu-id="2ca54-121">Non applicable</span><span class="sxs-lookup"><span data-stu-id="2ca54-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="2ca54-122">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2ca54-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ca54-123">False</span><span class="sxs-lookup"><span data-stu-id="2ca54-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ca54-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2ca54-124">See also</span></span>

- [<span data-ttu-id="2ca54-125">Applications</span><span class="sxs-lookup"><span data-stu-id="2ca54-125">Apps</span></span>](apps.md)
- [<span data-ttu-id="2ca54-126">Métadonnées</span><span class="sxs-lookup"><span data-stu-id="2ca54-126">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="2ca54-127">Manifeste</span><span class="sxs-lookup"><span data-stu-id="2ca54-127">Manifest</span></span>](manifest.md)
- [<span data-ttu-id="2ca54-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2ca54-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

