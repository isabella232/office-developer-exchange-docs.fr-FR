---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: L’élément ContactsView définit une recherche d’éléments de contact en fonction des noms d’affichage alphabétiques.
ms.openlocfilehash: 23c3fe13c44cdd0e5a054ecb3378bc3d633e55aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463817"
---
# <a name="contactsview"></a><span data-ttu-id="f9cd0-103">ContactsView</span><span class="sxs-lookup"><span data-stu-id="f9cd0-103">ContactsView</span></span>

<span data-ttu-id="f9cd0-104">L’élément **ContactsView** définit une recherche d’éléments de contact en fonction des noms d’affichage alphabétiques.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="f9cd0-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="f9cd0-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="f9cd0-106">ContactsView</span><span class="sxs-lookup"><span data-stu-id="f9cd0-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="f9cd0-107">**ContactsViewType**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f9cd0-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f9cd0-108">Attributes and elements</span></span>

<span data-ttu-id="f9cd0-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9cd0-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="f9cd0-110">Attributes</span></span>

|<span data-ttu-id="f9cd0-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-111">**Attribute**</span></span>|<span data-ttu-id="f9cd0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9cd0-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="f9cd0-114">Décrit le nombre maximal de résultats à renvoyer dans la réponse [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="f9cd0-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="f9cd0-115">**InitialName**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-115">**InitialName**</span></span> <br/> |<span data-ttu-id="f9cd0-116">Définit le premier nom de la liste de contacts à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="f9cd0-117">Si le nom d’origine spécifié ne figure pas dans la liste de contacts, le nom alphabétique suivant défini par le contexte culturel est renvoyé, sauf si le nom suivant vient après **FinalName**.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="f9cd0-118">Si l’attribut **InitialName** est omis, la réponse contient une liste de contacts qui commence par le prénom dans la liste des contacts.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="f9cd0-119">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="f9cd0-120">**FinalName**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-120">**FinalName**</span></span> <br/> |<span data-ttu-id="f9cd0-121">Définit le nom de famille de la liste de contacts à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="f9cd0-122">Si l’attribut **FinalName** est omis, la réponse contiendra tous les contacts suivants dans l’ordre de tri spécifié.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="f9cd0-123">Si le nom final spécifié ne figure pas dans la liste de contacts, le nom alphabétique suivant défini par le contexte culturel est exclu.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="f9cd0-124">Par exemple, si FinalName = « nom », mais que le nom ne figure pas dans la liste de contacts, les contacts dont le nom d’affichage est « name1 » ne seront pas inclus.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="f9cd0-125">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f9cd0-126">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f9cd0-126">Child elements</span></span>

<span data-ttu-id="f9cd0-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9cd0-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f9cd0-128">Parent elements</span></span>

|<span data-ttu-id="f9cd0-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-129">**Element**</span></span>|<span data-ttu-id="f9cd0-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9cd0-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9cd0-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="f9cd0-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="f9cd0-132">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="f9cd0-133">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f9cd0-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9cd0-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="f9cd0-134">Remarks</span></span>

<span data-ttu-id="f9cd0-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="f9cd0-136">Exemple</span><span class="sxs-lookup"><span data-stu-id="f9cd0-136">Example</span></span>

<span data-ttu-id="f9cd0-137">L’exemple de requête suivant montre comment rechercher les trois premiers contacts en commençant par le contact dont le nom d’affichage est Barbara Mayer.</span><span class="sxs-lookup"><span data-stu-id="f9cd0-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="f9cd0-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f9cd0-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9cd0-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f9cd0-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f9cd0-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f9cd0-140">Schema Name</span></span>  <br/> |<span data-ttu-id="f9cd0-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f9cd0-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f9cd0-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f9cd0-142">Validation File</span></span>  <br/> |<span data-ttu-id="f9cd0-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f9cd0-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f9cd0-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f9cd0-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9cd0-145">False</span><span class="sxs-lookup"><span data-stu-id="f9cd0-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9cd0-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9cd0-146">See also</span></span>

- [<span data-ttu-id="f9cd0-147">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="f9cd0-147">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="f9cd0-148">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="f9cd0-148">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

