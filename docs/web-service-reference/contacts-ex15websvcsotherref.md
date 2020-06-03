---
title: Contacts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contacts
api_type:
- schema
ms.assetid: 0cc67cdf-9707-45e7-92c6-fa83a016cdbe
description: L’élément contacts contient la liste des contacts associés à une tâche.
ms.openlocfilehash: c2b7bbadd494081a3e47b7b6c489218fab31d574
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458389"
---
# <a name="contacts"></a><span data-ttu-id="89eb0-103">Contacts</span><span class="sxs-lookup"><span data-stu-id="89eb0-103">Contacts</span></span>

<span data-ttu-id="89eb0-104">L’élément **contacts** contient la liste des contacts associés à une tâche.</span><span class="sxs-lookup"><span data-stu-id="89eb0-104">The **Contacts** element contains a list of contacts that are associated with a task.</span></span> 
  
```xml
<Contacts>
   <String/>
</Contacts>
```

 <span data-ttu-id="89eb0-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="89eb0-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89eb0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89eb0-106">Attributes and elements</span></span>

<span data-ttu-id="89eb0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89eb0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89eb0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="89eb0-108">Attributes</span></span>

<span data-ttu-id="89eb0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="89eb0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89eb0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89eb0-110">Child elements</span></span>

|<span data-ttu-id="89eb0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89eb0-111">**Element**</span></span>|<span data-ttu-id="89eb0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="89eb0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89eb0-113">String</span><span class="sxs-lookup"><span data-stu-id="89eb0-113">String</span></span>](string.md) <br/> |<span data-ttu-id="89eb0-114">Représente une liste de noms de contacts séparés par des virgules.</span><span class="sxs-lookup"><span data-stu-id="89eb0-114">Represents a comma-separated list of contact names.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89eb0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89eb0-115">Parent elements</span></span>

|<span data-ttu-id="89eb0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89eb0-116">**Element**</span></span>|<span data-ttu-id="89eb0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="89eb0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89eb0-118">Tâche</span><span class="sxs-lookup"><span data-stu-id="89eb0-118">Task</span></span>](task.md) <br/> |<span data-ttu-id="89eb0-119">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="89eb0-119">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89eb0-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="89eb0-120">Remarks</span></span>

<span data-ttu-id="89eb0-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="89eb0-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89eb0-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89eb0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89eb0-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89eb0-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89eb0-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89eb0-124">Schema name</span></span>  <br/> |<span data-ttu-id="89eb0-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="89eb0-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="89eb0-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89eb0-126">Validation file</span></span>  <br/> |<span data-ttu-id="89eb0-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89eb0-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89eb0-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89eb0-128">Can be empty</span></span>  <br/> |<span data-ttu-id="89eb0-129">False</span><span class="sxs-lookup"><span data-stu-id="89eb0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89eb0-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89eb0-130">See also</span></span>



- [<span data-ttu-id="89eb0-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89eb0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

