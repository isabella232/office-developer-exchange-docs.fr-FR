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
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467948"
---
# <a name="resolvenames"></a><span data-ttu-id="2b45d-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="2b45d-103">ResolveNames</span></span>

<span data-ttu-id="2b45d-104">L’élément **ResolveNames** définit une demande de résolution de noms ambigus.</span><span class="sxs-lookup"><span data-stu-id="2b45d-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="2b45d-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="2b45d-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b45d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2b45d-106">Attributes and elements</span></span>

<span data-ttu-id="2b45d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2b45d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b45d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2b45d-108">Attributes</span></span>

|<span data-ttu-id="2b45d-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="2b45d-109">**Attribute**</span></span>|<span data-ttu-id="2b45d-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b45d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b45d-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="2b45d-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="2b45d-112">Indique si les détails du contact complet pour les contacts publics pour un nom résolu sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="2b45d-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="2b45d-113">Cet attribut est requis pour les contacts publics.</span><span class="sxs-lookup"><span data-stu-id="2b45d-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="2b45d-114">Cette valeur n’affecte pas les contacts privés et les listes de distribution privées, pour lesquelles [ItemId](itemid.md) est toujours renvoyé.</span><span class="sxs-lookup"><span data-stu-id="2b45d-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="2b45d-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="2b45d-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="2b45d-116">Identifie l’ordre et l’étendue d’une recherche ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="2b45d-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="2b45d-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="2b45d-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="2b45d-118">Identifie le jeu de propriétés renvoyé pour les contacts.</span><span class="sxs-lookup"><span data-stu-id="2b45d-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="2b45d-119">Cet attribut a été introduit dans Exchange Server 2010 Service Pack 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="2b45d-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="2b45d-120">Valeurs d’attribut ReturnFullContactData</span><span class="sxs-lookup"><span data-stu-id="2b45d-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="2b45d-121">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2b45d-121">**Value**</span></span>|<span data-ttu-id="2b45d-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b45d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b45d-123">True</span><span class="sxs-lookup"><span data-stu-id="2b45d-123">True</span></span>  <br/> |<span data-ttu-id="2b45d-124">Les détails du contact complet pour les contacts publics sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="2b45d-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="2b45d-125">Faux</span><span class="sxs-lookup"><span data-stu-id="2b45d-125">False</span></span>  <br/> |<span data-ttu-id="2b45d-126">Les détails du contact complet pour les contacts publics ne sont pas renvoyés.</span><span class="sxs-lookup"><span data-stu-id="2b45d-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="2b45d-127">Valeurs de l’attribut SearchScope</span><span class="sxs-lookup"><span data-stu-id="2b45d-127">SearchScope attribute values</span></span>

|<span data-ttu-id="2b45d-128">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2b45d-128">**Value**</span></span>|<span data-ttu-id="2b45d-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b45d-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b45d-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="2b45d-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="2b45d-131">Seul le service d’annuaire Active Directory fait l’objet d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="2b45d-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="2b45d-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="2b45d-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="2b45d-133">Active Directory est recherché en premier, puis les dossiers de contacts qui sont spécifiés dans la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.</span><span class="sxs-lookup"><span data-stu-id="2b45d-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="2b45d-134">Contacts</span><span class="sxs-lookup"><span data-stu-id="2b45d-134">Contacts</span></span>  <br/> |<span data-ttu-id="2b45d-135">Seuls les dossiers de contacts identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés.</span><span class="sxs-lookup"><span data-stu-id="2b45d-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="2b45d-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="2b45d-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="2b45d-137">Les dossiers de contacts identifiés par la propriété [ParentFolderIds](parentfolderids.md) sont recherchés en premier, puis Active Directory est recherché.</span><span class="sxs-lookup"><span data-stu-id="2b45d-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="2b45d-138">Valeurs d’attribut ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="2b45d-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="2b45d-139">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="2b45d-139">**Value**</span></span>|<span data-ttu-id="2b45d-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b45d-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b45d-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="2b45d-141">IdOnly</span></span>  <br/> |<span data-ttu-id="2b45d-142">La propriété de l’identificateur d’élément de contact est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="2b45d-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="2b45d-143">Par défaut</span><span class="sxs-lookup"><span data-stu-id="2b45d-143">Default</span></span>  <br/> |<span data-ttu-id="2b45d-144">L’ensemble par défaut des propriétés d’élément de contact est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="2b45d-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="2b45d-145">Pour plus d’informations, consultez la rubrique [Shapes Response in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2b45d-145">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="2b45d-146">AllProperties</span><span class="sxs-lookup"><span data-stu-id="2b45d-146">AllProperties</span></span>  <br/> |<span data-ttu-id="2b45d-147">Le jeu AllProperties de propriétés d’élément de contact est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="2b45d-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="2b45d-148">Pour plus d’informations, consultez la rubrique [Shapes Response in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2b45d-148">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2b45d-149">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2b45d-149">Child elements</span></span>

|<span data-ttu-id="2b45d-150">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b45d-150">**Element**</span></span>|<span data-ttu-id="2b45d-151">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b45d-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b45d-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="2b45d-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="2b45d-153">Contient un tableau d’identificateurs de dossiers de contacts qui seraient recherchés si l’attribut **SearchScope** est défini sur ActiveDirectoryContacts, contacts ou ContactsActiveDirectory.</span><span class="sxs-lookup"><span data-stu-id="2b45d-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="2b45d-154">Le tableau ParentFolderIds ne peut contenir qu’un seul identificateur de dossier de contact.</span><span class="sxs-lookup"><span data-stu-id="2b45d-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="2b45d-155">Si l’élément **ParentFolderIds** n’est pas présent, le dossier de contacts par défaut est recherché.</span><span class="sxs-lookup"><span data-stu-id="2b45d-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="2b45d-156">L’identificateur de dossier peut être utilisé pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="2b45d-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="2b45d-157">Les recherches Active Directory sont effectuées à l’aide de listes de contrôle d’accès (ACL).</span><span class="sxs-lookup"><span data-stu-id="2b45d-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="2b45d-158">Certains utilisateurs ne disposent pas des droits pour afficher certains objets Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2b45d-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="2b45d-159">Cet élément est facultatif.</span><span class="sxs-lookup"><span data-stu-id="2b45d-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2b45d-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="2b45d-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="2b45d-161">Contient le nom d’un contact ou d’une liste de distribution à résoudre.</span><span class="sxs-lookup"><span data-stu-id="2b45d-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b45d-162">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2b45d-162">Parent elements</span></span>

<span data-ttu-id="2b45d-163">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b45d-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b45d-164">Remarques</span><span class="sxs-lookup"><span data-stu-id="2b45d-164">Remarks</span></span>

<span data-ttu-id="2b45d-165">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b45d-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b45d-166">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2b45d-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b45d-167">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2b45d-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2b45d-168">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2b45d-168">Schema name</span></span>  <br/> |<span data-ttu-id="2b45d-169">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2b45d-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2b45d-170">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2b45d-170">Validation file</span></span>  <br/> |<span data-ttu-id="2b45d-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2b45d-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2b45d-172">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2b45d-172">Can be empty</span></span>  <br/> |<span data-ttu-id="2b45d-173">False</span><span class="sxs-lookup"><span data-stu-id="2b45d-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b45d-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b45d-174">See also</span></span>



[<span data-ttu-id="2b45d-175">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="2b45d-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="2b45d-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="2b45d-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="2b45d-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="2b45d-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="2b45d-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2b45d-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2b45d-179">Utilisation de la résolution de noms</span><span class="sxs-lookup"><span data-stu-id="2b45d-179">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

