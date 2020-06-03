---
title: Opération UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: L’opération UpdateItem est utilisée pour modifier les propriétés d’un élément existant dans la Banque d’Exchange.
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459390"
---
# <a name="updateitem-operation"></a><span data-ttu-id="b0c2f-103">Opération UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b0c2f-103">UpdateItem operation</span></span>

<span data-ttu-id="b0c2f-104">L’opération **UpdateItem** est utilisée pour modifier les propriétés d’un élément existant dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b0c2f-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="b0c2f-105">Remarks</span></span>

<span data-ttu-id="b0c2f-106">Vous pouvez effectuer trois actions de mise à jour de base sur un élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="b0c2f-107">Le tableau suivant répertorie les actions que vous pouvez effectuer.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="b0c2f-108">**Action**</span><span class="sxs-lookup"><span data-stu-id="b0c2f-108">**Action**</span></span>|<span data-ttu-id="b0c2f-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0c2f-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b0c2f-110">Ajout</span><span class="sxs-lookup"><span data-stu-id="b0c2f-110">Append</span></span>  <br/> |<span data-ttu-id="b0c2f-111">Ajoute des données à une propriété existante.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-111">Adds data to an existing property.</span></span> <span data-ttu-id="b0c2f-112">Cette action conserve les données actuelles.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-112">This action preserves the current data.</span></span> <span data-ttu-id="b0c2f-113">Append ne s’applique pas à toutes les propriétés.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="b0c2f-114">Set</span><span class="sxs-lookup"><span data-stu-id="b0c2f-114">Set</span></span>  <br/> |<span data-ttu-id="b0c2f-115">Remplace les données d’une propriété si la propriété contient des données, ou crée la propriété et définit sa valeur si la propriété n’existe pas.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="b0c2f-116">L’action set n’est applicable qu’aux propriétés accessibles en écriture.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="b0c2f-117">Supprimer</span><span class="sxs-lookup"><span data-stu-id="b0c2f-117">Delete</span></span>  <br/> |<span data-ttu-id="b0c2f-118">Supprime une propriété d’un élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-118">Removes a property from an item.</span></span> <span data-ttu-id="b0c2f-119">Cela diffère de la définition d’une propriété sur une valeur vide.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="b0c2f-120">Lorsque cette action est terminée, la propriété n’existe pas pour l’élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="b0c2f-121">La méthode Delete n’est applicable qu’aux propriétés accessibles en écriture.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="b0c2f-122">Un appel **UpdateItem** peut être utilisé pour modifier un ou plusieurs éléments, ainsi qu’une ou plusieurs propriétés sur chaque élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="b0c2f-123">L’élément [itemChanges](itemchanges.md) contient toutes les modifications qui doivent être effectuées dans le cadre de cet appel.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="b0c2f-124">L’élément [ItemChange,](itemchange.md) , enfant de l’élément [itemChanges](itemchanges.md) , représente les modifications à effectuer sur un seul élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="b0c2f-125">L’élément [ItemChange,](itemchange.md) contient un ensemble d’actions de mise à jour qui peuvent être effectuées sur un seul élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="b0c2f-126">Ces modifications sont contenues dans l’élément [Updates (élément)](updates-item.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c2f-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="b0c2f-127">L’élément [ItemId](itemid.md) identifie l’élément à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="b0c2f-128">Pour mettre à jour plusieurs propriétés sur un élément, un [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) doit être fourni pour chaque propriété nécessitant la mise à jour.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b0c2f-129">Les actions de mise à jour sont appliquées dans l’ordre dans lequel elles sont spécifiées.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="b0c2f-130">Pour chaque modification, vous devez spécifier le chemin d’accès de la propriété à modifier et une représentation de cet élément avec sa nouvelle valeur.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="b0c2f-131">L’action de suppression est légèrement différente dans la mesure où seul le chemin de la propriété à supprimer est requis.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="b0c2f-132">Pour les actions Set et Append, le chemin d’accès spécifié doit faire référence à la même propriété que celle définie dans la représentation de l’élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="b0c2f-133">Si elles diffèrent, une erreur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="b0c2f-134">L’opération **UpdateItem** peut définir l’heure de [début](start.md) et de [fin](end-ex15websvcsotherref.md) d’un élément de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="b0c2f-135">Dans une requête **UpdateItem** , l’heure de [début](start.md) peut être définie sans définir également l’heure de [fin](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c2f-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="b0c2f-136">Cela peut entraîner une erreur si l’heure de [début](start.md) est postérieure à l’heure de [fin](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="b0c2f-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="b0c2f-137">N’oubliez pas que les applications clientes doivent ajuster l’heure de [fin](end-ex15websvcsotherref.md) lorsque l’heure de [début](start.md) est modifiée afin de conserver la durée.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="b0c2f-138">Lorsqu’un seul élément de calendrier est mis à jour pour devenir un élément de calendrier principal périodique, la propriété [MeetingTimeZone](meetingtimezone.md) doit être définie par l’opération **UpdateItem** afin de conserver le fuseau horaire d’origine de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="b0c2f-139">Exemple de requête SetItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="b0c2f-140">Description</span><span class="sxs-lookup"><span data-stu-id="b0c2f-140">Description</span></span>

<span data-ttu-id="b0c2f-141">L’exemple de requête **UpdateItem** suivant montre comment définir la propriété Sensitivity sur un élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b0c2f-142">Code</span><span class="sxs-lookup"><span data-stu-id="b0c2f-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b0c2f-143">Commentaires</span><span class="sxs-lookup"><span data-stu-id="b0c2f-143">Comments</span></span>

<span data-ttu-id="b0c2f-144">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="b0c2f-145">Éléments de requête SetItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-145">SetItemField Request Elements</span></span>

<span data-ttu-id="b0c2f-146">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="b0c2f-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b0c2f-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b0c2f-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="b0c2f-148">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="b0c2f-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="b0c2f-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="b0c2f-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="b0c2f-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="b0c2f-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b0c2f-151">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="b0c2f-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="b0c2f-152">SetItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="b0c2f-153">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b0c2f-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="b0c2f-154">Message</span><span class="sxs-lookup"><span data-stu-id="b0c2f-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b0c2f-155">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="b0c2f-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="b0c2f-156">Exemple de requête AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="b0c2f-157">Description</span><span class="sxs-lookup"><span data-stu-id="b0c2f-157">Description</span></span>

<span data-ttu-id="b0c2f-158">L’exemple de requête **UpdateItem** suivant montre comment ajouter du texte à la propriété Body sur un élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b0c2f-159">Code</span><span class="sxs-lookup"><span data-stu-id="b0c2f-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b0c2f-160">Commentaires</span><span class="sxs-lookup"><span data-stu-id="b0c2f-160">Comments</span></span>

<span data-ttu-id="b0c2f-161">Les propriétés suivantes prennent en charge l’action Append :</span><span class="sxs-lookup"><span data-stu-id="b0c2f-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="b0c2f-162">**message : ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="b0c2f-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="b0c2f-163">**élément : Body**</span><span class="sxs-lookup"><span data-stu-id="b0c2f-163">**item:Body**</span></span>
    
- <span data-ttu-id="b0c2f-164">Toutes les propriétés du destinataire et de la collection de participants</span><span class="sxs-lookup"><span data-stu-id="b0c2f-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="b0c2f-165">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="b0c2f-166">Éléments de requête AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="b0c2f-167">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="b0c2f-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b0c2f-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b0c2f-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="b0c2f-169">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="b0c2f-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="b0c2f-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="b0c2f-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="b0c2f-171">ItemId</span><span class="sxs-lookup"><span data-stu-id="b0c2f-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b0c2f-172">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="b0c2f-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="b0c2f-173">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="b0c2f-174">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b0c2f-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="b0c2f-175">Message</span><span class="sxs-lookup"><span data-stu-id="b0c2f-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b0c2f-176">Corps</span><span class="sxs-lookup"><span data-stu-id="b0c2f-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="b0c2f-177">Exemple de requête DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="b0c2f-178">Description</span><span class="sxs-lookup"><span data-stu-id="b0c2f-178">Description</span></span>

<span data-ttu-id="b0c2f-179">L’exemple de requête **UpdateItem** suivant montre comment supprimer une propriété sur un élément.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b0c2f-180">Code</span><span class="sxs-lookup"><span data-stu-id="b0c2f-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b0c2f-181">Commentaires</span><span class="sxs-lookup"><span data-stu-id="b0c2f-181">Comments</span></span>

<span data-ttu-id="b0c2f-182">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="b0c2f-183">Éléments de requête DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="b0c2f-184">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="b0c2f-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b0c2f-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b0c2f-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="b0c2f-186">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="b0c2f-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="b0c2f-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="b0c2f-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="b0c2f-188">ItemId</span><span class="sxs-lookup"><span data-stu-id="b0c2f-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b0c2f-189">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="b0c2f-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="b0c2f-190">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="b0c2f-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="b0c2f-191">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b0c2f-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="b0c2f-192">Exemple de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="b0c2f-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="b0c2f-193">Description</span><span class="sxs-lookup"><span data-stu-id="b0c2f-193">Description</span></span>

<span data-ttu-id="b0c2f-194">L’exemple suivant montre une réponse réussie à une demande **UpdateItem** .</span><span class="sxs-lookup"><span data-stu-id="b0c2f-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b0c2f-195">Code</span><span class="sxs-lookup"><span data-stu-id="b0c2f-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b0c2f-196">Commentaires</span><span class="sxs-lookup"><span data-stu-id="b0c2f-196">Comments</span></span>

<span data-ttu-id="b0c2f-197">L’identificateur d’élément et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="b0c2f-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="b0c2f-198">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="b0c2f-198">Successful response elements</span></span>

<span data-ttu-id="b0c2f-199">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="b0c2f-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b0c2f-200">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b0c2f-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b0c2f-201">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="b0c2f-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="b0c2f-202">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b0c2f-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b0c2f-203">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b0c2f-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="b0c2f-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b0c2f-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b0c2f-205">Items</span><span class="sxs-lookup"><span data-stu-id="b0c2f-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="b0c2f-206">Message</span><span class="sxs-lookup"><span data-stu-id="b0c2f-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b0c2f-207">ItemId</span><span class="sxs-lookup"><span data-stu-id="b0c2f-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="b0c2f-208">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0c2f-208">See also</span></span>



[<span data-ttu-id="b0c2f-209">Opération UpdateItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="b0c2f-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="b0c2f-210">Opération UpdateItem (contact)</span><span class="sxs-lookup"><span data-stu-id="b0c2f-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="b0c2f-211">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b0c2f-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="b0c2f-212">Updating Contacts</span><span class="sxs-lookup"><span data-stu-id="b0c2f-212">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="b0c2f-213">Mise à jour des tâches</span><span class="sxs-lookup"><span data-stu-id="b0c2f-213">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

