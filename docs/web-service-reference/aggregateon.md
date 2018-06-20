---
title: AggregateOn
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AggregateOn
api_type:
- schema
ms.assetid: 9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb
description: L’élément AggregateOn représente la propriété qui est utilisée pour déterminer l’ordre des éléments regroupés pour un jeu de résultats FindItem groupé.
ms.openlocfilehash: fe14de23e6a4c90d826200cae927427acfccc3c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755189"
---
# <a name="aggregateon"></a><span data-ttu-id="dd178-103">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="dd178-103">AggregateOn</span></span>

<span data-ttu-id="dd178-104">L’élément **AggregateOn** représente la propriété qui est utilisée pour déterminer l’ordre des éléments regroupés pour un jeu de résultats FindItem groupé.</span><span class="sxs-lookup"><span data-stu-id="dd178-104">The **AggregateOn** element represents the property that is used to determine the order of grouped items for a grouped FindItem result set.</span></span> 
  
- [<span data-ttu-id="dd178-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="dd178-105">FindItem</span></span>](finditem.md)  
- [<span data-ttu-id="dd178-106">GroupBy</span><span class="sxs-lookup"><span data-stu-id="dd178-106">GroupBy</span></span>](groupby.md)
- [<span data-ttu-id="dd178-107">AggregateOn</span><span class="sxs-lookup"><span data-stu-id="dd178-107">AggregateOn</span></span>](aggregateon.md)
  
```xml
<AggregateOn>
   <FieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <IndexedFieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <ExtendedFieldURI/>
</AggregateOn>
```
 
<span data-ttu-id="dd178-108">**AggregateOnType**</span><span class="sxs-lookup"><span data-stu-id="dd178-108">**AggregateOnType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dd178-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dd178-109">Attributes and elements</span></span>

<span data-ttu-id="dd178-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dd178-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd178-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="dd178-111">Attributes</span></span>

|<span data-ttu-id="dd178-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="dd178-112">**Attribute**</span></span>|<span data-ttu-id="dd178-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="dd178-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd178-114">**Aggregate**</span><span class="sxs-lookup"><span data-stu-id="dd178-114">**Aggregate**</span></span> <br/> | <span data-ttu-id="dd178-115">Indique la valeur minimale ou maximale de la propriété identifiée par l’élément [FieldURI](fielduri.md) qui est utilisé pour classer les groupes d’éléments.</span><span class="sxs-lookup"><span data-stu-id="dd178-115">Indicates the maximum or minimum value of the property identified by the [FieldURI](fielduri.md) element that is used for ordering the groups of items.</span></span><br/><br/><span data-ttu-id="dd178-116">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="dd178-116">The following are the possible values:</span></span>  <br/><br/><span data-ttu-id="dd178-117">-Minimum</span><span class="sxs-lookup"><span data-stu-id="dd178-117">- Minimum</span></span>  <br/><span data-ttu-id="dd178-118">-Maximum</span><span class="sxs-lookup"><span data-stu-id="dd178-118">- Maximum</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dd178-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dd178-119">Child elements</span></span>

|<span data-ttu-id="dd178-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dd178-120">**Element**</span></span>|<span data-ttu-id="dd178-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="dd178-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd178-122">FieldURI</span><span class="sxs-lookup"><span data-stu-id="dd178-122">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="dd178-123">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="dd178-123">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="dd178-124">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="dd178-124">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="dd178-125">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="dd178-125">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="dd178-126">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="dd178-126">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="dd178-127">Identifie les propriétés MAPI étendues pour obtenir, définir ou créer.</span><span class="sxs-lookup"><span data-stu-id="dd178-127">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd178-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dd178-128">Parent elements</span></span>

|<span data-ttu-id="dd178-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dd178-129">**Element**</span></span>|<span data-ttu-id="dd178-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="dd178-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd178-131">GroupBy</span><span class="sxs-lookup"><span data-stu-id="dd178-131">GroupBy</span></span>](groupby.md) <br/> |<span data-ttu-id="dd178-132">Spécifie les regroupements arbitraires pour les requêtes FindItem.</span><span class="sxs-lookup"><span data-stu-id="dd178-132">Specifies arbitrary groupings for FindItem queries.</span></span>  <br/> <span data-ttu-id="dd178-133">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/FindItem/GroupBy`</span><span class="sxs-lookup"><span data-stu-id="dd178-133">The following is the XPath expression to this element:  `/FindItem/GroupBy`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd178-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="dd178-134">Remarks</span></span>

<span data-ttu-id="dd178-135">L' [opération FindItem](finditem-operation.md) peut renvoyer des résultats groupés.</span><span class="sxs-lookup"><span data-stu-id="dd178-135">The [FindItem operation](finditem-operation.md) can return grouped results.</span></span> <span data-ttu-id="dd178-136">Dans les résultats groupés, tous les éléments qui ont la même valeur pour une propriété de regroupement donné sont rassemblées et présentés en tant qu’enfants de ce groupe.</span><span class="sxs-lookup"><span data-stu-id="dd178-136">Within grouped results, all items that have the same value for a given grouping property are gathered together and presented as children of that group.</span></span> <span data-ttu-id="dd178-137">Par exemple, si vous regroupez par expéditeur, tous les messages électroniques sont organisés en groupes distincts selon qu’ils soient à partir de l’expéditeur A, B de l’expéditeur et ainsi de suite.</span><span class="sxs-lookup"><span data-stu-id="dd178-137">For example, if you group by sender, all e-mails are organized into separate groups based on whether they are from sender A, sender B, and so on.</span></span> <span data-ttu-id="dd178-138">Ces groupes sont les enfants du groupe de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="dd178-138">These groups are children of the sender group.</span></span> 
  
<span data-ttu-id="dd178-139">Chacun des groupes au sein du groupe de l’expéditeur constituée une collection d’éléments, tels que les messages électroniques réels dont provient chaque expéditeur.</span><span class="sxs-lookup"><span data-stu-id="dd178-139">Each of the groups within the sender group contains a collection of items, such as the actual e-mails that came from each sender.</span></span> <span data-ttu-id="dd178-140">Vous pouvez utiliser l’élément de [l’ordre de tri](sortorder.md) pour trier les éléments dans un groupe.</span><span class="sxs-lookup"><span data-stu-id="dd178-140">You can use the [SortOrder](sortorder.md) element to sort the items within a group.</span></span> <span data-ttu-id="dd178-141">Pour trier les groupes en fonction des valeurs de propriété d’un élément, toutefois, vous devez utiliser l’agrégation.</span><span class="sxs-lookup"><span data-stu-id="dd178-141">To sort the groups based on an item's property values, however, you must use aggregation.</span></span> 
  
<span data-ttu-id="dd178-142">Avec l’agrégation, l’ordre des groupes est basé sur une propriété spécifique des éléments au sein du groupe.</span><span class="sxs-lookup"><span data-stu-id="dd178-142">With aggregation, the order of groups is based on a specific property of the items within the group.</span></span> <span data-ttu-id="dd178-143">Lorsque vous utilisez l’agrégation de tri des éléments dans un groupe, vous devez identifier une propriété représentant à utiliser pour trier les groupes.</span><span class="sxs-lookup"><span data-stu-id="dd178-143">When you use aggregation to sort items within a group, you must identify a representative property by which to sort the groups.</span></span> <span data-ttu-id="dd178-144">Vous pouvez utiliser l’élément **AggregateOn** pour spécifier la propriété représentative.</span><span class="sxs-lookup"><span data-stu-id="dd178-144">You can use the **AggregateOn** element to specify the representative property.</span></span> 
  
<span data-ttu-id="dd178-145">Lorsqu’une propriété représentant est identifiée, l’attribut **d’agrégation** est utilisé pour indiquer si les groupes sont triés en fonction de la valeur maximale ou la valeur minimale de la propriété identifiée.</span><span class="sxs-lookup"><span data-stu-id="dd178-145">When a representative property is identified, the **Aggregate** attribute is used to indicate whether the groups are sorted according to the maximum or the minimum value of the identified property.</span></span> <span data-ttu-id="dd178-146">Si l’attribut **global** est défini sur Maximum, les groupes sont triés commençant par la plus grande valeur de la propriété **AggregateOn** .</span><span class="sxs-lookup"><span data-stu-id="dd178-146">If the **Aggregate** attribute is set to Maximum, the groups are sorted beginning with the largest value for the **AggregateOn** property.</span></span> <span data-ttu-id="dd178-147">Si l’attribut **global** est défini au Minimum, les groupes sont triés commençant par la plus petite valeur de la propriété **AggregateOn** .</span><span class="sxs-lookup"><span data-stu-id="dd178-147">If the **Aggregate** attribute is set to Minimum, the groups are sorted beginning with the smallest value for the **AggregateOn** property.</span></span> 
  
<span data-ttu-id="dd178-148">Par exemple, si vous souhaitez émettre une requête groupée FindItem, regrouper par expéditeur, mais vous souhaitez classer les groupes de sorte que le groupe avec le message électronique plus récent est en haut, vous pouvez regrouper par expéditeur et AGREGAT sur date/heure de réception avec un **regroupement** attribut de Maximum.</span><span class="sxs-lookup"><span data-stu-id="dd178-148">For example, if you want to issue a FindItem grouped query, grouping by sender, but you want to order the groups so that the group with the most recent e-mail message is on top, you can group by sender and aggregate on date/time received with an **Aggregate** attribute of Maximum.</span></span> 
  
<span data-ttu-id="dd178-149">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dd178-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="dd178-150">Exemple</span><span class="sxs-lookup"><span data-stu-id="dd178-150">Example</span></span>

<span data-ttu-id="dd178-151">L’exemple suivant montre un groupées FindItem demande et réponse.</span><span class="sxs-lookup"><span data-stu-id="dd178-151">The following example shows a grouped FindItem request and response.</span></span> <span data-ttu-id="dd178-152">L’exemple illustre une demande pour renvoyer des éléments regroupés par la propriété **ConversationTopic** .</span><span class="sxs-lookup"><span data-stu-id="dd178-152">The example shows a request to return items grouped by the **ConversationTopic** property.</span></span> <span data-ttu-id="dd178-153">Deux groupes, A et B, sont retournés dans l’ordre décroissant selon la valeur maximale de la propriété [DateTimeReceived](datetimereceived.md) .</span><span class="sxs-lookup"><span data-stu-id="dd178-153">Two groups, A and B, are returned in descending order based on the maximum value of the [DateTimeReceived](datetimereceived.md) property.</span></span> 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="message:ConversationTopic"/>
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AdditionalProperties>    
      </ItemShape>
      <IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="20" Offset="0"/>
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="message:ConversationTopic"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
<!-- EXAMPLE RESPONSE -->
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>B</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAH=" ChangeKey="CQAAABY" />
                    <t:DateTimeReceived>2006-09-14T23:59:18Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnAHR=" ChangeKey="CQAAAw" />
                    <t:DateTimeReceived>2006-09-15T00:00:24Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnA==" ChangeKey="CQAAJXT" />
                    <t:DateTimeReceived>2006-09-15T00:22:45Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>A</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAAA==" ChangeKey="CQCJNe" />
                    <t:DateTimeReceived>2006-09-14T23:56:12Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQWgAA==" ChangeKey="CQAACJV6" />
                    <t:DateTimeReceived>2006-09-14T23:57:33Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAAA==" ChangeKey="CQA6CJXw" />
                    <t:DateTimeReceived>2006-09-15T00:23:31Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="dd178-154">Pour trier les éléments dans un groupe, utilisez l’élément [SortOrder](sortorder.md) .</span><span class="sxs-lookup"><span data-stu-id="dd178-154">To sort the items in a group, use the [SortOrder](sortorder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="dd178-155">Les identificateurs de l’élément et les touches de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="dd178-155">The item identifiers and change keys have been shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="dd178-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dd178-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd178-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dd178-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd178-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dd178-158">Schema Name</span></span>  <br/> |<span data-ttu-id="dd178-159">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dd178-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd178-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dd178-160">Validation File</span></span>  <br/> |<span data-ttu-id="dd178-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd178-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd178-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dd178-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd178-163">False</span><span class="sxs-lookup"><span data-stu-id="dd178-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd178-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dd178-164">See also</span></span>

- [<span data-ttu-id="dd178-165">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="dd178-165">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="dd178-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dd178-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="dd178-167">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="dd178-167">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

