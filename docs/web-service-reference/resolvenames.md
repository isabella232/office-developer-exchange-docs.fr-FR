---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: L’élément ResolveNames définit une demande de résolution de noms ambigus.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829172"
---
# <a name="resolvenames"></a><span data-ttu-id="000b2-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="000b2-103">ResolveNames</span></span>

<span data-ttu-id="000b2-104">L’élément **ResolveNames** définit une demande de résolution de noms ambigus.</span><span class="sxs-lookup"><span data-stu-id="000b2-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="000b2-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="000b2-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="000b2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="000b2-106">Attributes and elements</span></span>

<span data-ttu-id="000b2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="000b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="000b2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="000b2-108">Attributes</span></span>

|<span data-ttu-id="000b2-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="000b2-109">**Attribute**</span></span>|<span data-ttu-id="000b2-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="000b2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000b2-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="000b2-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="000b2-112">Indique si les détails de contact pour les contacts publics pour un nom résolu sont retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="000b2-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="000b2-113">Cet attribut est requis pour les contacts publics.</span><span class="sxs-lookup"><span data-stu-id="000b2-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="000b2-114">Cette valeur n’affecte pas les contacts privés et les listes de distribution privée, pour laquelle [ItemId](itemid.md) est toujours renvoyée.</span><span class="sxs-lookup"><span data-stu-id="000b2-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="000b2-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="000b2-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="000b2-116">Identifie le sens et l’étendue de la recherche ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="000b2-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="000b2-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="000b2-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="000b2-118">Identifie la propriété la valeur renvoyée pour les contacts.</span><span class="sxs-lookup"><span data-stu-id="000b2-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="000b2-119">Cet attribut est une nouveauté dans Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="000b2-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="000b2-120">Valeurs des attributs ReturnFullContactData</span><span class="sxs-lookup"><span data-stu-id="000b2-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="000b2-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="000b2-121">**Value**</span></span>|<span data-ttu-id="000b2-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="000b2-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000b2-123">True</span><span class="sxs-lookup"><span data-stu-id="000b2-123">True</span></span>  <br/> |<span data-ttu-id="000b2-124">Plus d’informations de contacts pour les contacts publics sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="000b2-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="000b2-125">Faux</span><span class="sxs-lookup"><span data-stu-id="000b2-125">False</span></span>  <br/> |<span data-ttu-id="000b2-126">Plus d’informations de contacts pour les contacts publics ne sont pas renvoyés.</span><span class="sxs-lookup"><span data-stu-id="000b2-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="000b2-127">Valeurs d’attribut SearchScope</span><span class="sxs-lookup"><span data-stu-id="000b2-127">SearchScope attribute values</span></span>

|<span data-ttu-id="000b2-128">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="000b2-128">**Value**</span></span>|<span data-ttu-id="000b2-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="000b2-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000b2-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="000b2-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="000b2-131">Recherche uniquement le service d’annuaire Active Directory est effectuée.</span><span class="sxs-lookup"><span data-stu-id="000b2-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="000b2-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="000b2-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="000b2-133">Active Directory est recherché en premier, puis les dossiers de contacts qui sont spécifiés dans la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.</span><span class="sxs-lookup"><span data-stu-id="000b2-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="000b2-134">Contacts</span><span class="sxs-lookup"><span data-stu-id="000b2-134">Contacts</span></span>  <br/> |<span data-ttu-id="000b2-135">Seuls les dossiers de contacts qui sont identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.</span><span class="sxs-lookup"><span data-stu-id="000b2-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="000b2-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="000b2-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="000b2-137">Dossiers de contacts qui sont identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés en premier, et puis Active Directory est recherché.</span><span class="sxs-lookup"><span data-stu-id="000b2-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="000b2-138">Valeurs des attributs ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="000b2-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="000b2-139">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="000b2-139">**Value**</span></span>|<span data-ttu-id="000b2-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="000b2-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="000b2-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="000b2-141">IdOnly</span></span>  <br/> |<span data-ttu-id="000b2-142">La propriété d’élément de contact identificateur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="000b2-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="000b2-143">Default (Défaut)</span><span class="sxs-lookup"><span data-stu-id="000b2-143">Default</span></span>  <br/> |<span data-ttu-id="000b2-144">L’ensemble par défaut des propriétés de l’élément de contact est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="000b2-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="000b2-145">Pour plus d’informations, voir [formes réponse dans EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="000b2-145">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="000b2-146">AllProperties</span><span class="sxs-lookup"><span data-stu-id="000b2-146">AllProperties</span></span>  <br/> |<span data-ttu-id="000b2-147">L’ensemble de AllProperties des propriétés de l’élément de contact sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="000b2-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="000b2-148">Pour plus d’informations, voir [formes réponse dans EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="000b2-148">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="000b2-149">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="000b2-149">Child elements</span></span>

|<span data-ttu-id="000b2-150">**Élément**</span><span class="sxs-lookup"><span data-stu-id="000b2-150">**Element**</span></span>|<span data-ttu-id="000b2-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="000b2-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="000b2-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="000b2-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="000b2-153">Contient un tableau d’identificateurs de dossier de contacts qui doit être recherché si l’attribut **SearchScope** est défini sur ActiveDirectoryContacts, Contacts ou ContactsActiveDirectory.</span><span class="sxs-lookup"><span data-stu-id="000b2-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="000b2-154">Le tableau ParentFolderIds ne peut contenir qu’un identificateur unique de dossier de contacts.</span><span class="sxs-lookup"><span data-stu-id="000b2-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="000b2-155">Si l’élément **ParentFolderIds** n’est pas présent, le dossier Contacts par défaut est recherché.</span><span class="sxs-lookup"><span data-stu-id="000b2-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="000b2-156">L’identificateur de dossier peut être utilisé pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="000b2-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="000b2-157">Recherches Active Directory sont effectuées à l’aide de listes de contrôle d’accès (ACL).</span><span class="sxs-lookup"><span data-stu-id="000b2-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="000b2-158">Certains utilisateurs n’est peut-être pas les droits à voir certains objets Active Directory.</span><span class="sxs-lookup"><span data-stu-id="000b2-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="000b2-159">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="000b2-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="000b2-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="000b2-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="000b2-161">Contient le nom d’une liste de contacts ou de distribution à résoudre.</span><span class="sxs-lookup"><span data-stu-id="000b2-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="000b2-162">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="000b2-162">Parent elements</span></span>

<span data-ttu-id="000b2-163">Aucun.</span><span class="sxs-lookup"><span data-stu-id="000b2-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="000b2-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="000b2-164">Remarks</span></span>

<span data-ttu-id="000b2-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="000b2-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="000b2-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="000b2-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="000b2-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="000b2-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="000b2-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="000b2-168">Schema name</span></span>  <br/> |<span data-ttu-id="000b2-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="000b2-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="000b2-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="000b2-170">Validation file</span></span>  <br/> |<span data-ttu-id="000b2-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="000b2-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="000b2-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="000b2-172">Can be empty</span></span>  <br/> |<span data-ttu-id="000b2-173">False</span><span class="sxs-lookup"><span data-stu-id="000b2-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="000b2-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="000b2-174">See also</span></span>



[<span data-ttu-id="000b2-175">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="000b2-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="000b2-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="000b2-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="000b2-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="000b2-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="000b2-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="000b2-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="000b2-179">À l’aide de la résolution de noms</span><span class="sxs-lookup"><span data-stu-id="000b2-179">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

