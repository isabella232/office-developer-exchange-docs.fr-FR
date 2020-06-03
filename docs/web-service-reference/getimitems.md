---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: L’élément de requête GetImItems définit une demande pour obtenir des informations sur les groupes de messagerie instantanée et les personnes de contacts de messagerie instantanée spécifiés.
ms.openlocfilehash: e3973cbbf800ffe91472b9c733c4d4a927b91c9f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456450"
---
# <a name="getimitems"></a><span data-ttu-id="710fd-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="710fd-103">GetImItems</span></span>

<span data-ttu-id="710fd-104">L’élément de requête **GetImItems** définit une demande pour obtenir des informations sur les groupes de messagerie instantanée et les personnes de contacts de messagerie instantanée spécifiés.</span><span class="sxs-lookup"><span data-stu-id="710fd-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="710fd-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="710fd-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="710fd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="710fd-106">Attributes and elements</span></span>

<span data-ttu-id="710fd-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="710fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="710fd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="710fd-108">Attributes</span></span>

<span data-ttu-id="710fd-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="710fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="710fd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="710fd-110">Child elements</span></span>

<span data-ttu-id="710fd-111">[ContactIds](contactids.md)  |  [ID](groupids.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="710fd-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="710fd-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="710fd-112">Parent elements</span></span>

<span data-ttu-id="710fd-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="710fd-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="710fd-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="710fd-114">Remarks</span></span>

<span data-ttu-id="710fd-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="710fd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="710fd-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="710fd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="710fd-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="710fd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="710fd-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="710fd-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="710fd-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="710fd-119">Schema name</span></span>  <br/> |<span data-ttu-id="710fd-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="710fd-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="710fd-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="710fd-121">Validation file</span></span>  <br/> |<span data-ttu-id="710fd-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="710fd-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="710fd-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="710fd-123">Can be empty</span></span>  <br/> ||
   

