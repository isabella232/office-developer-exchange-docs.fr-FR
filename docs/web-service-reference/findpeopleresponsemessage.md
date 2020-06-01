---
title: FindPeopleResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba686738-e654-404d-ab54-83c71d030350
description: L’élément FindPeopleResponseMessage spécifie le message de réponse pour une demande FindPeople.
ms.openlocfilehash: 5a2ce7b8643fff9d4a93b62459638d3a99605c98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466373"
---
# <a name="findpeopleresponsemessage"></a><span data-ttu-id="61cc7-103">FindPeopleResponseMessage</span><span class="sxs-lookup"><span data-stu-id="61cc7-103">FindPeopleResponseMessage</span></span>

<span data-ttu-id="61cc7-104">L’élément **FindPeopleResponseMessage** spécifie le message de réponse pour une demande **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="61cc7-104">The **FindPeopleResponseMessage** element specifies the response message for a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <People/>
   <TotalNumberOfPeopleInView/>
</FindPeopleResponseMessage>
```

 <span data-ttu-id="61cc7-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="61cc7-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61cc7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="61cc7-106">Attributes and elements</span></span>

<span data-ttu-id="61cc7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="61cc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61cc7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="61cc7-108">Attributes</span></span>

<span data-ttu-id="61cc7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="61cc7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61cc7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="61cc7-110">Child elements</span></span>

<span data-ttu-id="61cc7-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [Personnes](people.md)  |  [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span><span class="sxs-lookup"><span data-stu-id="61cc7-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [People](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61cc7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="61cc7-112">Parent elements</span></span>

[<span data-ttu-id="61cc7-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="61cc7-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="61cc7-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="61cc7-114">Remarks</span></span>

<span data-ttu-id="61cc7-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="61cc7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="61cc7-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="61cc7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61cc7-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="61cc7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61cc7-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="61cc7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="61cc7-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="61cc7-119">Schema name</span></span>  <br/> |<span data-ttu-id="61cc7-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="61cc7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="61cc7-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="61cc7-121">Validation file</span></span>  <br/> |<span data-ttu-id="61cc7-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="61cc7-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="61cc7-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="61cc7-123">Can be empty</span></span>  <br/> |<span data-ttu-id="61cc7-124">false</span><span class="sxs-lookup"><span data-stu-id="61cc7-124">false</span></span>  <br/> |
   

