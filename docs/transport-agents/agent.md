---
title: agent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Dernière modification : 17 septembre 2015'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755112"
---
# <a name="agent"></a><span data-ttu-id="66624-103">agent</span><span class="sxs-lookup"><span data-stu-id="66624-103">agent</span></span>
  
<span data-ttu-id="66624-104">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="66624-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="66624-105">L’élément de **l’agent** contient des informations de configuration sur un agent installé.</span><span class="sxs-lookup"><span data-stu-id="66624-105">The **agent** element contains configuration information about an installed agent.</span></span> 
  
- [<span data-ttu-id="66624-106">configuration</span><span class="sxs-lookup"><span data-stu-id="66624-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="66624-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="66624-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="66624-108">agentList</span><span class="sxs-lookup"><span data-stu-id="66624-108">agentList</span></span>](agentlist.md)
- [<span data-ttu-id="66624-109">agent</span><span class="sxs-lookup"><span data-stu-id="66624-109">agent</span></span>](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

<span data-ttu-id="66624-110">**type_agent (type complexe)**</span><span class="sxs-lookup"><span data-stu-id="66624-110">**agentType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="66624-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="66624-111">Attributes and elements</span></span>

<span data-ttu-id="66624-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="66624-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66624-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="66624-113">Attributes</span></span>

|<span data-ttu-id="66624-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="66624-114">**Attribute**</span></span>|<span data-ttu-id="66624-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="66624-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66624-116">**nom**</span><span class="sxs-lookup"><span data-stu-id="66624-116">**name**</span></span> <br/> |<span data-ttu-id="66624-117">Le nom spécifié lors de l’agent a été installé.</span><span class="sxs-lookup"><span data-stu-id="66624-117">The name that was specified when the agent was installed.</span></span> <span data-ttu-id="66624-118">Cet attribut requiert une valeur de chaîne non vide qui contient un maximum de 64 caractères.</span><span class="sxs-lookup"><span data-stu-id="66624-118">This attribute requires a nonempty string value that contains a maximum of 64 characters.</span></span>  <br/> |
|<span data-ttu-id="66624-119">**baseType**</span><span class="sxs-lookup"><span data-stu-id="66624-119">**baseType**</span></span> <br/> |<span data-ttu-id="66624-120">Le nom complet, y compris l’espace de noms de la classe qui dérive de l’agent.</span><span class="sxs-lookup"><span data-stu-id="66624-120">The full name, including the namespace, of the class from which the agent derives.</span></span> <span data-ttu-id="66624-121">Cet attribut requiert une valeur de chaîne non vide qui contient au moins un caractère.</span><span class="sxs-lookup"><span data-stu-id="66624-121">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="66624-122">**classFactory**</span><span class="sxs-lookup"><span data-stu-id="66624-122">**classFactory**</span></span> <br/> |<span data-ttu-id="66624-123">Le nom complet, y compris l’espace de noms de la classe qui implémente la fabrique de l’agent qui crée des instances de l’agent.</span><span class="sxs-lookup"><span data-stu-id="66624-123">The full name, including the namespace, of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="66624-124">Cet attribut doit contenir le nom qualifié complet de la classe qui implémente la fabrique de l’agent qui crée des instances de l’agent.</span><span class="sxs-lookup"><span data-stu-id="66624-124">This attribute must contain the fully qualified name of the class that implements the agent factory that creates instances of the agent.</span></span> <span data-ttu-id="66624-125">Cette classe doit dériver de la classe [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) ou de [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="66624-125">This class must derive from either the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) or [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span>  <br/> |
|<span data-ttu-id="66624-126">**assemblyPath**</span><span class="sxs-lookup"><span data-stu-id="66624-126">**assemblyPath**</span></span> <br/> |<span data-ttu-id="66624-127">Chemin d’accès complet, y compris le nom de fichier de l’assembly qui contient le code pour l’agent.</span><span class="sxs-lookup"><span data-stu-id="66624-127">The fully qualified path, including the file name, of the assembly that contains the code for the agent.</span></span> <span data-ttu-id="66624-128">Cet attribut requiert une valeur de chaîne non vide qui contient au moins un caractère.</span><span class="sxs-lookup"><span data-stu-id="66624-128">This attribute requires a nonempty string value that contains at least one character.</span></span>  <br/> |
|<span data-ttu-id="66624-129">**activé**</span><span class="sxs-lookup"><span data-stu-id="66624-129">**enabled**</span></span> <br/> |<span data-ttu-id="66624-130">Une valeur de type Boolean qui indique si l’agent est activé.</span><span class="sxs-lookup"><span data-stu-id="66624-130">A Boolean value that indicates whether the agent is enabled.</span></span> <span data-ttu-id="66624-131">La valeur est **true** si l’agent est activé ; dans le cas contraire, la valeur est **false**.</span><span class="sxs-lookup"><span data-stu-id="66624-131">The value is **true** if the agent is enabled; otherwise, the value is **false**.</span></span> <span data-ttu-id="66624-132">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="66624-132">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66624-133">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="66624-133">Child elements</span></span>

<span data-ttu-id="66624-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="66624-134">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66624-135">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="66624-135">Parent elements</span></span>

|<span data-ttu-id="66624-136">**Élément**</span><span class="sxs-lookup"><span data-stu-id="66624-136">**Element**</span></span>|<span data-ttu-id="66624-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="66624-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66624-138">agentList</span><span class="sxs-lookup"><span data-stu-id="66624-138">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="66624-139">Contient un élément de **l’agent** pour chaque agent installé.</span><span class="sxs-lookup"><span data-stu-id="66624-139">Contains an **agent** element for each installed agent.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="66624-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="66624-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66624-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="66624-141">Namespace</span></span>  <br/> |<span data-ttu-id="66624-142">Ce fichier ne définit pas un espace de noms.</span><span class="sxs-lookup"><span data-stu-id="66624-142">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="66624-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="66624-143">Schema Name</span></span>  <br/> |<span data-ttu-id="66624-144">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="66624-144">Not available.</span></span>  <br/> |
|<span data-ttu-id="66624-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="66624-145">Validation File</span></span>  <br/> |<span data-ttu-id="66624-146">N’est pas disponible.</span><span class="sxs-lookup"><span data-stu-id="66624-146">Not available.</span></span>  <br/> |
|<span data-ttu-id="66624-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="66624-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="66624-148">Faux</span><span class="sxs-lookup"><span data-stu-id="66624-148">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66624-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="66624-149">See also</span></span>

- [<span data-ttu-id="66624-150">Éléments du fichier de configuration agents pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="66624-150">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

