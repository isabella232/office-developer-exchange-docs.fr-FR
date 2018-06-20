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
description: L’élément ContactsView définit une recherche des éléments de contact basées sur des noms d’affichage alphabétiques.
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755578"
---
# <a name="contactsview"></a><span data-ttu-id="dcfe6-103">ContactsView</span><span class="sxs-lookup"><span data-stu-id="dcfe6-103">ContactsView</span></span>

<span data-ttu-id="dcfe6-104">L’élément **ContactsView** définit une recherche des éléments de contact basées sur des noms d’affichage alphabétiques.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="dcfe6-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="dcfe6-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="dcfe6-106">ContactsView</span><span class="sxs-lookup"><span data-stu-id="dcfe6-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="dcfe6-107">**ContactsViewType**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dcfe6-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dcfe6-108">Attributes and elements</span></span>

<span data-ttu-id="dcfe6-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcfe6-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="dcfe6-110">Attributes</span></span>

|<span data-ttu-id="dcfe6-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-111">**Attribute**</span></span>|<span data-ttu-id="dcfe6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dcfe6-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="dcfe6-114">Indique le nombre maximal de résultats à retourner dans la réponse [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="dcfe6-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="dcfe6-115">**InitialName**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-115">**InitialName**</span></span> <br/> |<span data-ttu-id="dcfe6-116">Définit le premier nom dans la liste des contacts à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="dcfe6-117">Si le nom initial spécifié n’est pas dans la liste des contacts, le nom suivant alphabétique tel que défini par le contexte culturel s’afficheront, sauf si le nom suivant vient après **FinalName**.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="dcfe6-118">Si l’attribut **InitialName** est omis, la réponse contient une liste des contacts qui commence par le premier nom dans la liste des contacts.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="dcfe6-119">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="dcfe6-120">**FinalName**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-120">**FinalName**</span></span> <br/> |<span data-ttu-id="dcfe6-121">Définit le nom de famille dans la liste des contacts à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="dcfe6-122">Si l’attribut **FinalName** est omis, la réponse contient tous les contacts suivants dans l’ordre de tri spécifié.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="dcfe6-123">Si le nom de la dernière spécifié n’est pas dans la liste des contacts, le nom suivant alphabétique tel que défini par le contexte culturel sera exclu.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="dcfe6-124">Par exemple, si FinalName = « Name », mais nom n’est pas dans la liste de contacts, contacts disposant d’affichent les noms de nom1 ou nom ne seront pas inclus.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="dcfe6-125">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="dcfe6-126">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dcfe6-126">Child elements</span></span>

<span data-ttu-id="dcfe6-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dcfe6-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dcfe6-128">Parent elements</span></span>

|<span data-ttu-id="dcfe6-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-129">**Element**</span></span>|<span data-ttu-id="dcfe6-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcfe6-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcfe6-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="dcfe6-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="dcfe6-132">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="dcfe6-133">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="dcfe6-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dcfe6-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="dcfe6-134">Remarks</span></span>

<span data-ttu-id="dcfe6-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="dcfe6-136">Exemple</span><span class="sxs-lookup"><span data-stu-id="dcfe6-136">Example</span></span>

<span data-ttu-id="dcfe6-137">Une demande de l’exemple suivant montre comment rechercher les trois premiers contacts commençant par le contact dont le nom complet de Kelly Rollin.</span><span class="sxs-lookup"><span data-stu-id="dcfe6-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="dcfe6-138">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dcfe6-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcfe6-139">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dcfe6-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dcfe6-140">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dcfe6-140">Schema Name</span></span>  <br/> |<span data-ttu-id="dcfe6-141">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="dcfe6-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dcfe6-142">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dcfe6-142">Validation File</span></span>  <br/> |<span data-ttu-id="dcfe6-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dcfe6-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dcfe6-144">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dcfe6-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="dcfe6-145">False</span><span class="sxs-lookup"><span data-stu-id="dcfe6-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcfe6-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dcfe6-146">See also</span></span>

- [<span data-ttu-id="dcfe6-147">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="dcfe6-147">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="dcfe6-148">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="dcfe6-148">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

