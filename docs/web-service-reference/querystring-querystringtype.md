---
title: QueryString (QueryStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- QueryString
api_type:
- schema
ms.assetid: cadbf9a5-b87e-4d7f-b488-b76fb0ee7150
description: L’élément de la chaîne de requête contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).
ms.openlocfilehash: 410405638b3f8628dc589049873cfea1f153310c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828943"
---
# <a name="querystring-querystringtype"></a><span data-ttu-id="b2fa7-103">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-103">QueryString (QueryStringType)</span></span>

<span data-ttu-id="b2fa7-104">L’élément de la **chaîne de requête** contient une chaîne de requête de boîte aux lettres basée sur la syntaxe de requête avancée (AQS).</span><span class="sxs-lookup"><span data-stu-id="b2fa7-104">The **QueryString** element contains a mailbox query string based on Advanced Query Syntax (AQS).</span></span> 
  
```XML
<QueryString/>
```

 <span data-ttu-id="b2fa7-105">**QueryStringType**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-105">**QueryStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2fa7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b2fa7-106">Attributes and elements</span></span>

<span data-ttu-id="b2fa7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2fa7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b2fa7-108">Attributes</span></span>

|<span data-ttu-id="b2fa7-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-109">**Attribute**</span></span>|<span data-ttu-id="b2fa7-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b2fa7-111">ResetCache</span><span class="sxs-lookup"><span data-stu-id="b2fa7-111">ResetCache</span></span>  <br/> |<span data-ttu-id="b2fa7-112">Indique que le cache doit être réinitialisé.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-112">Indicates that the cache should be reset.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-113">ReturnDeletedItems</span><span class="sxs-lookup"><span data-stu-id="b2fa7-113">ReturnDeletedItems</span></span>  <br/> |<span data-ttu-id="b2fa7-114">Indique que les éléments supprimés doivent être retournées.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-114">Indicates that deleted items should be returned.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-115">ReturnHighlightTerms</span><span class="sxs-lookup"><span data-stu-id="b2fa7-115">ReturnHighlightTerms</span></span>  <br/> |<span data-ttu-id="b2fa7-116">Indique que la mise en surbrillance des termes doivent être retournés.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-116">Indicates that highlighted terms should be returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b2fa7-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b2fa7-117">Child elements</span></span>

<span data-ttu-id="b2fa7-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2fa7-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b2fa7-119">Parent elements</span></span>

|<span data-ttu-id="b2fa7-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-120">**Element**</span></span>|<span data-ttu-id="b2fa7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2fa7-122">FindItem</span><span class="sxs-lookup"><span data-stu-id="b2fa7-122">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="b2fa7-123">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-123">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="b2fa7-124">Voici l’expression XPath pour cet élément : /FindItem.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-124">The following is the XPath expression to this element: /FindItem.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b2fa7-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b2fa7-125">Text value</span></span>

<span data-ttu-id="b2fa7-126">La valeur de texte d’élément **QueryString** représente une requête de boîte aux lettres qui est effectuée à l’aide d’un sous-ensemble de [La syntaxe de requête avancée (AQS)](http://msdn.microsoft.com/fr-fr/library/aa965711%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b2fa7-126">The **QueryString** element text value represents a mailbox query that is made by using a subset of [Advanced Query Syntax (AQS)](http://msdn.microsoft.com/fr-fr/library/aa965711%28VS.85%29.aspx).</span></span> <span data-ttu-id="b2fa7-127">Voir la section Notes pour plus d’informations sur les options de syntaxe prise en charge pour les chaînes de requête.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-127">See the remarks section for information about the supported syntax options for query strings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2fa7-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="b2fa7-128">Remarks</span></span>

<span data-ttu-id="b2fa7-129">Dans Exchange Server 2010, cet élément est un type de chaîne de schéma XML.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-129">In Exchange Server 2010, this element is an XML schema string type.</span></span> <span data-ttu-id="b2fa7-130">Dans les versions d’Exchange commençant par Exchange Server 2013, notamment Exchange Online, le type de cet élément est **QueryStringType**.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-130">In versions of Exchange starting with Exchange Server 2013, including Exchange Online, the type for this element is **QueryStringType**.</span></span> <span data-ttu-id="b2fa7-131">Cette modification n’arrête pas tous les clients existants, car elle ajoute trois nouveaux attributs facultatifs.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-131">This change does not break any existing clients because it adds three new optional attributes.</span></span> 
  
<span data-ttu-id="b2fa7-132">L’élément **QueryString** exclut l’utilisation des restrictions EWS.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-132">The **QueryString** element excludes the use of EWS restrictions.</span></span> <span data-ttu-id="b2fa7-133">AQS dans EWS prend en charge trois types de restrictions : word phase restriction, restriction de plage de date et restriction de type de message.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-133">AQS in EWS supports three types of restrictions: word phase restriction, date range restriction, and message type restriction.</span></span> <span data-ttu-id="b2fa7-134">Les tableaux suivants répertorient les propriétés de recherche prises en charge pour chaque type de restriction.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-134">The following tables list the supported search properties for each restriction type.</span></span> 
  
<span data-ttu-id="b2fa7-135">**Restriction de phase de Word**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-135">**Word phase restriction**</span></span>

|<span data-ttu-id="b2fa7-136">**Propriété**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-136">**Property**</span></span>|<span data-ttu-id="b2fa7-137">**Exemple**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-137">**Example**</span></span>|<span data-ttu-id="b2fa7-138">**Fonction**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-138">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2fa7-139">from</span><span class="sxs-lookup"><span data-stu-id="b2fa7-139">from</span></span>  <br/> |<span data-ttu-id="b2fa7-140">À partir de : Olivier</span><span class="sxs-lookup"><span data-stu-id="b2fa7-140">From:Dean</span></span>  <br/> <span data-ttu-id="b2fa7-141">À partir de : « Olivier Halstead »</span><span class="sxs-lookup"><span data-stu-id="b2fa7-141">From:"Dean Halstead"</span></span>  <br/> |<span data-ttu-id="b2fa7-142">Rechercher des éléments envoyés à partir d’Olivier.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-142">Search items sent from Dean.</span></span>  <br/> <span data-ttu-id="b2fa7-143">Rechercher des éléments envoyés à partir de Dean Halstead.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-143">Search items sent from Dean Halstead.</span></span> <span data-ttu-id="b2fa7-144">L’expéditeur doit être exactement « Olivier Halstead ».</span><span class="sxs-lookup"><span data-stu-id="b2fa7-144">The sender must be exactly "Dean Halstead".</span></span>  <br/> |
|<span data-ttu-id="b2fa7-145">et utilisez à la place</span><span class="sxs-lookup"><span data-stu-id="b2fa7-145">to</span></span>  <br/> |<span data-ttu-id="b2fa7-146">À : Olivier</span><span class="sxs-lookup"><span data-stu-id="b2fa7-146">To:Dean</span></span>  <br/> |<span data-ttu-id="b2fa7-147">Rechercher des éléments envoyés à Olivier.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-147">Search items sent to Dean.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-148">cc</span><span class="sxs-lookup"><span data-stu-id="b2fa7-148">cc</span></span>  <br/> |<span data-ttu-id="b2fa7-149">Cc:Dean</span><span class="sxs-lookup"><span data-stu-id="b2fa7-149">Cc:Dean</span></span>  <br/> |<span data-ttu-id="b2fa7-150">Rechercher des éléments avec Olivier sur la ligne Cc.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-150">Search for items with Dean on the Cc line.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-151">bcc</span><span class="sxs-lookup"><span data-stu-id="b2fa7-151">bcc</span></span>  <br/> |<span data-ttu-id="b2fa7-152">Bcc:Dean</span><span class="sxs-lookup"><span data-stu-id="b2fa7-152">Bcc:Dean</span></span>  <br/> |<span data-ttu-id="b2fa7-153">Rechercher des éléments avec Olivier sur la ligne Cci.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-153">Search for items with Dean on the Bcc line.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-154">Participants</span><span class="sxs-lookup"><span data-stu-id="b2fa7-154">Participants</span></span>  <br/> |<span data-ttu-id="b2fa7-155">Participants : Olivier</span><span class="sxs-lookup"><span data-stu-id="b2fa7-155">Participants:Dean</span></span>  <br/> |<span data-ttu-id="b2fa7-156">Recherche d’éléments dont l’olivier dans l’à, Cc ou Cci champs.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-156">Search for items with Dean in the To, Cc, or Bcc fields.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-157">Objet</span><span class="sxs-lookup"><span data-stu-id="b2fa7-157">Subject</span></span>  <br/> |<span data-ttu-id="b2fa7-158">Objet : produit</span><span class="sxs-lookup"><span data-stu-id="b2fa7-158">Subject:product</span></span>  <br/> <span data-ttu-id="b2fa7-159">Objet :(product development)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-159">Subject:(product development)</span></span>  <br/> <span data-ttu-id="b2fa7-160">Objet : « développement de produit »</span><span class="sxs-lookup"><span data-stu-id="b2fa7-160">Subject:"product development"</span></span>  <br/> |<span data-ttu-id="b2fa7-161">Rechercher des éléments avec le produit dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-161">Search for items with product in the subject.</span></span>  <br/> <span data-ttu-id="b2fa7-162">Rechercher des éléments avec des produits et de développement dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-162">Search for items with product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-163">Corps</span><span class="sxs-lookup"><span data-stu-id="b2fa7-163">Body</span></span>  <br/> <span data-ttu-id="b2fa7-164">Content</span><span class="sxs-lookup"><span data-stu-id="b2fa7-164">Content</span></span>  <br/> |<span data-ttu-id="b2fa7-165">Corps : progression</span><span class="sxs-lookup"><span data-stu-id="b2fa7-165">Body:progress</span></span>  <br/> <span data-ttu-id="b2fa7-166">Contenu : progression</span><span class="sxs-lookup"><span data-stu-id="b2fa7-166">Content:progress</span></span>  <br/> |<span data-ttu-id="b2fa7-167">Rechercher des éléments avec l’avancement dans le corps.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-167">Search for items with progress in the body.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-168">Pièce jointe</span><span class="sxs-lookup"><span data-stu-id="b2fa7-168">Attachment</span></span>  <br/> |<span data-ttu-id="b2fa7-169">Pièce jointe : état</span><span class="sxs-lookup"><span data-stu-id="b2fa7-169">Attachment:report</span></span>  <br/> |<span data-ttu-id="b2fa7-170">Recherche d’éléments dont l’état dans le corps de fichier ou nom de fichier des pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-170">Search for items with report in the attachment file name or file body.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-171">(la propriété n’est pas spécifiée)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-171">(property is not specified)</span></span>  <br/> |<span data-ttu-id="b2fa7-172">Développement de produits</span><span class="sxs-lookup"><span data-stu-id="b2fa7-172">Product Development</span></span>  <br/> |<span data-ttu-id="b2fa7-173">Rechercher des éléments qui contiennent des produits et développement dans toutes les propriétés de phase de word.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-173">Search for items that contain both product and development in all word phase properties.</span></span>  <br/> |
   
<span data-ttu-id="b2fa7-174">Correspondance de restriction de phase Word est toujours la casse.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-174">Word phase restriction match is always case insensitive.</span></span> <span data-ttu-id="b2fa7-175">Restriction de phase Word prend en charge deux types de correspondance : correspondance de préfixe ou correspondance exacte.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-175">Word phase restriction supports two match types: prefix match or exact match.</span></span> <span data-ttu-id="b2fa7-176">Correspondance de préfixe est le comportement de correspondance par défaut.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-176">Prefix match is the default match behavior.</span></span> <span data-ttu-id="b2fa7-177">Si vous souhaitez une correspondance exacte, utilisez des guillemets doubles.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-177">If you want exact match, use double quotes.</span></span> <span data-ttu-id="b2fa7-178">Par exemple, l’objet : « produit » correspond à « produit » mais pas « production » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-178">For example, subject:"product" matches 'product' but not 'production' in the subject.</span></span> <span data-ttu-id="b2fa7-179">Plusieurs mots dans des guillemets doubles restreindre les phases de word et leur ordre.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-179">Multiple words in double quotes restrict both word phases and their order.</span></span> <span data-ttu-id="b2fa7-180">Par exemple, « produit win » correspond à la seule « win produit », pas « produit Windows 95 » ou « produit de win ».</span><span class="sxs-lookup"><span data-stu-id="b2fa7-180">For example "win product" matches only 'win product', not 'win95 product' or 'product of win'.</span></span> <span data-ttu-id="b2fa7-181">Vous pouvez utiliser un astérisque (\*) pour définir une correspondance de préfixe avec commande restreints.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-181">You can use an asterisk (\*) to define a prefix match with order restricted.</span></span> <span data-ttu-id="b2fa7-182">Par exemple, « win produit »\* correspond à « produit Windows 95 », « ligne de production windows » mais pas « windows nouveau produit » ou « produit de win ».</span><span class="sxs-lookup"><span data-stu-id="b2fa7-182">For example, "win product"\* matches 'win95 product', 'windows production line' but not 'windows new product' or 'product of win'.</span></span> <span data-ttu-id="b2fa7-183">Vous pouvez rechercher tous les messages envoyés à partir d’ou à un domaine.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-183">You can search all messages sent from or to a domain.</span></span> <span data-ttu-id="b2fa7-184">Par exemple, from:"@hotmail.com » renvoie tous les messages envoyés à partir de hotmail.com.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-184">For example, from:"@hotmail.com" returns all messages sent from hotmail.com.</span></span>
  
<span data-ttu-id="b2fa7-185">Le tableau suivant décrit les restrictions de plage de date.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-185">The following table describes date range restrictions.</span></span>
  
<span data-ttu-id="b2fa7-186">**Restriction de plage de date**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-186">**Date range restriction**</span></span>

|<span data-ttu-id="b2fa7-187">**Propriété**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-187">**Property**</span></span>|<span data-ttu-id="b2fa7-188">**Exemple**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-188">**Example**</span></span>|<span data-ttu-id="b2fa7-189">**Fonction**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-189">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2fa7-190">Envoyé</span><span class="sxs-lookup"><span data-stu-id="b2fa7-190">Sent</span></span>  <br/> |<span data-ttu-id="b2fa7-191">Envoyés : semaine dernière</span><span class="sxs-lookup"><span data-stu-id="b2fa7-191">Sent:last week</span></span>  <br/> <span data-ttu-id="b2fa7-192">Envoyés : 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="b2fa7-192">Sent:01/01/2001</span></span>  <br/> <span data-ttu-id="b2fa7-193">Sent:01/01/2001..01/15/2001</span><span class="sxs-lookup"><span data-stu-id="b2fa7-193">Sent:01/01/2001..01/15/2001</span></span>  <br/> |<span data-ttu-id="b2fa7-194">Recherche éléments envoyés la semaine dernière.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-194">Search items sent last week.</span></span>  <br/> <span data-ttu-id="b2fa7-195">Rechercher des éléments envoyés sur le 1er janvier 2001.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-195">Search items sent on January 1st, 2001.</span></span>  <br/> <span data-ttu-id="b2fa7-196">Rechercher des éléments envoyés entre le 1er janvier 2001 et le 15 janvier 2001.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-196">Search items sent between January 1st, 2001 and January 15th, 2001.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-197">Received</span><span class="sxs-lookup"><span data-stu-id="b2fa7-197">Received</span></span>  <br/> |<span data-ttu-id="b2fa7-198">Reçus : aujourd'hui</span><span class="sxs-lookup"><span data-stu-id="b2fa7-198">Received:today</span></span>  <br/> <span data-ttu-id="b2fa7-199">Reçus : 01/01/2001</span><span class="sxs-lookup"><span data-stu-id="b2fa7-199">Received:01/01/2001</span></span>  <br/> |<span data-ttu-id="b2fa7-200">Rechercher des éléments reçus dans la journée.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-200">Search items received today.</span></span>  <br/> <span data-ttu-id="b2fa7-201">Rechercher des éléments reçus sur le 1er janvier 2001.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-201">Search items received on January 1st, 2001.</span></span>  <br/> |
   
<span data-ttu-id="b2fa7-202">Les deux points (.) est un opérateur de plage.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-202">The two dots (..) is a range operator.</span></span> <span data-ttu-id="b2fa7-203">Il peut être utilisé pour définir une plage avec un point de départ et une date de fin.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-203">It can be used to define a range with a start and an end date.</span></span> <span data-ttu-id="b2fa7-204">Pour spécifier une date, vous pouvez utiliser des dates relatives.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-204">To specify a date, you can use relative dates.</span></span> <span data-ttu-id="b2fa7-205">Les dates relatives suivantes sont prises en charge :</span><span class="sxs-lookup"><span data-stu-id="b2fa7-205">The following relative dates are supported:</span></span>
  
- <span data-ttu-id="b2fa7-206">Dates relatives : aujourd'hui, demain, hier</span><span class="sxs-lookup"><span data-stu-id="b2fa7-206">Relative dates: Today, tomorrow, yesterday</span></span>
    
- <span data-ttu-id="b2fa7-207">Expressions de plusieurs dates relatives : cette semaine, le mois prochain, semaine dernière, au-delà de mois ou année</span><span class="sxs-lookup"><span data-stu-id="b2fa7-207">Multiword relative dates: This week, next month, last week, past month, or coming year</span></span>
    
- <span data-ttu-id="b2fa7-208">Jours : Dimanche, lundi, mardi, mercredi, jeudi, vendredi, samedi</span><span class="sxs-lookup"><span data-stu-id="b2fa7-208">Days: Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday</span></span>
    
- <span data-ttu-id="b2fa7-209">Janvier, février, mars, avril, mai, juin, juillet, août, septembre, octobre, novembre et décembre</span><span class="sxs-lookup"><span data-stu-id="b2fa7-209">January, February, March, April, May, June, July, August, September, October, November, December</span></span>
    
<span data-ttu-id="b2fa7-210">Le tableau suivant décrit les restrictions de type de message.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-210">The following table describes message type restrictions.</span></span> 
  
<span data-ttu-id="b2fa7-211">**Restriction de type de message**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-211">**Message type restriction**</span></span>

|<span data-ttu-id="b2fa7-212">**Propriété**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-212">**Property**</span></span>|<span data-ttu-id="b2fa7-213">**Exemple**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-213">**Example**</span></span>|<span data-ttu-id="b2fa7-214">**Fonction**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-214">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2fa7-215">Type</span><span class="sxs-lookup"><span data-stu-id="b2fa7-215">Kind</span></span>  <br/> |<span data-ttu-id="b2fa7-216">Type : tâches</span><span class="sxs-lookup"><span data-stu-id="b2fa7-216">Kind:tasks</span></span>  <br/> |<span data-ttu-id="b2fa7-217">Rechercher tous les éléments de tâche.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-217">Search all task items.</span></span>  <br/> |
   
<span data-ttu-id="b2fa7-218">AQS dans EWS utilise la propriété **Kind** pour spécifier le type de message.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-218">AQS in EWS uses the **Kind** property to specify the message type.</span></span> <span data-ttu-id="b2fa7-219">La propriété Kind peut être utilisée avec les types d’élément suivants :</span><span class="sxs-lookup"><span data-stu-id="b2fa7-219">The Kind property can be used with the following item types:</span></span> 
  
- <span data-ttu-id="b2fa7-220">email</span><span class="sxs-lookup"><span data-stu-id="b2fa7-220">email</span></span>
    
- <span data-ttu-id="b2fa7-221">réunions</span><span class="sxs-lookup"><span data-stu-id="b2fa7-221">meetings</span></span>
    
- <span data-ttu-id="b2fa7-222">tasks</span><span class="sxs-lookup"><span data-stu-id="b2fa7-222">tasks</span></span>
    
- <span data-ttu-id="b2fa7-223">notes</span><span class="sxs-lookup"><span data-stu-id="b2fa7-223">notes</span></span>
    
- <span data-ttu-id="b2fa7-224">documents</span><span class="sxs-lookup"><span data-stu-id="b2fa7-224">docs</span></span>
    
- <span data-ttu-id="b2fa7-225">feuilles</span><span class="sxs-lookup"><span data-stu-id="b2fa7-225">journals</span></span>
    
- <span data-ttu-id="b2fa7-226">contacts</span><span class="sxs-lookup"><span data-stu-id="b2fa7-226">contacts</span></span>
    
- <span data-ttu-id="b2fa7-227">messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="b2fa7-227">im</span></span>
    
<span data-ttu-id="b2fa7-228">Le tableau suivant décrit le regroupement logiques connecteurs.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-228">The following table describes grouping logical connectors.</span></span>
  
<span data-ttu-id="b2fa7-229">**Regroupement logiques connecteurs**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-229">**Grouping logical connectors**</span></span>

|<span data-ttu-id="b2fa7-230">**Connecteur**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-230">**Connector**</span></span>|<span data-ttu-id="b2fa7-231">**Exemple**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-231">**Example**</span></span>|<span data-ttu-id="b2fa7-232">**Fonction**</span><span class="sxs-lookup"><span data-stu-id="b2fa7-232">**Function**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2fa7-233">AND</span><span class="sxs-lookup"><span data-stu-id="b2fa7-233">AND</span></span>  <br/> |<span data-ttu-id="b2fa7-234">Objet : produit et subject : développement</span><span class="sxs-lookup"><span data-stu-id="b2fa7-234">Subject:product AND subject:development</span></span>  <br/> <span data-ttu-id="b2fa7-235">Objet :(product AND development)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-235">Subject:(product AND development)</span></span>  <br/> <span data-ttu-id="b2fa7-236">Objet :(product development)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-236">Subject:(product development)</span></span>  <br/> |<span data-ttu-id="b2fa7-237">Rechercher des éléments avec des produits et de développement dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-237">Search items with both product and development in the subject.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-238">OU</span><span class="sxs-lookup"><span data-stu-id="b2fa7-238">OR</span></span>  <br/> |<span data-ttu-id="b2fa7-239">Corps : projet ou corps : proposition</span><span class="sxs-lookup"><span data-stu-id="b2fa7-239">Body:project OR body:proposal</span></span>  <br/> <span data-ttu-id="b2fa7-240">Corps :(project OR proposal)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-240">Body:(project OR proposal)</span></span>  <br/> |<span data-ttu-id="b2fa7-241">Rechercher des éléments avec le produit ou de développement dans le corps.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-241">Search items with either product or development in the body.</span></span>  <br/> |
|<span data-ttu-id="b2fa7-242">NOT</span><span class="sxs-lookup"><span data-stu-id="b2fa7-242">NOT</span></span>  <br/> |<span data-ttu-id="b2fa7-243">PAS de corps : proposition</span><span class="sxs-lookup"><span data-stu-id="b2fa7-243">NOT body:proposal</span></span>  <br/> <span data-ttu-id="b2fa7-244">Corps :(NOT proposal)</span><span class="sxs-lookup"><span data-stu-id="b2fa7-244">Body:(NOT proposal)</span></span>  <br/> |<span data-ttu-id="b2fa7-245">Rechercher des messages sans proposition dans le corps.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-245">Search messages without proposal in the body.</span></span>  <br/> |
   
<span data-ttu-id="b2fa7-246">ET est toujours le connecteur par défaut.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-246">AND is always the default connector.</span></span> <span data-ttu-id="b2fa7-247">Par exemple, subject : projet et corps : proposition est le même que le corps : proposition de sujet : projet.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-247">For example, subject:project AND body:proposal is the same as subject:project body:proposal.</span></span> <span data-ttu-id="b2fa7-248">Connecteurs logiques respectent la casse.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-248">Logical connectors are case sensitive.</span></span> <span data-ttu-id="b2fa7-249">Par exemple, le corps :(project Or proposal) recherche des messages avec « projet », « ou » et « proposition' dans le corps au lieu de « projet » ou « proposition ».</span><span class="sxs-lookup"><span data-stu-id="b2fa7-249">For example, body:(project Or proposal) searches messages with 'project', 'or', and 'proposal' in the body instead of 'project' or 'proposal'.</span></span> <span data-ttu-id="b2fa7-250">Le signe plus (+) est équivalent à and.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-250">The plus symbol (+) is equivalent to AND.</span></span> <span data-ttu-id="b2fa7-251">Le symbole de trait d’union (-) est équivalente à ne pas.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-251">The hyphen symbol (-) is equivalent to NOT.</span></span> <span data-ttu-id="b2fa7-252">Par exemple, le corps :(project-proposal) recherche des messages avec « projet », mais sans 'proposition' dans le corps.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-252">For example, body:(project - proposal) searches messages with 'project' but without 'proposal' in the body.</span></span> 
  
<span data-ttu-id="b2fa7-253">La chaîne de requête peut également contenir les propriétés non indexées pour la recherche.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-253">The query string can also contain nonindexed properties for search.</span></span> <span data-ttu-id="b2fa7-254">Si la chaîne de requête contient les propriétés non indexées, la recherche peut effectuer une recherche Exchange sur les propriétés indexées et une banque de recherche sur les propriétés non indexées.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-254">If the query string contains nonindexed properties, the search might perform an Exchange search on the indexed properties and a store search on the nonindexed properties.</span></span> 
  
<span data-ttu-id="b2fa7-255">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-255">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="b2fa7-256">Exemple</span><span class="sxs-lookup"><span data-stu-id="b2fa7-256">Example</span></span>

<span data-ttu-id="b2fa7-257">L’exemple suivant montre une requête pour rechercher des messages dans la boîte de réception avec Autodiscover dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-257">The following example shows a request to search for messages in the Inbox with Autodiscover in the subject.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:Autodiscover</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b2fa7-258">L’exemple suivant montre une réponse positive à la demande.</span><span class="sxs-lookup"><span data-stu-id="b2fa7-258">The following example shows a successful response to the request.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" 
                        TotalItemsInView="5" 
                        IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkADEzOTExYjJkLTYx" ChangeKey="CQAAABY" />
                <t:Subject>How to use Autodiscover</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="element-information"></a><span data-ttu-id="b2fa7-259">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b2fa7-259">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2fa7-260">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b2fa7-260">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b2fa7-261">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b2fa7-261">Schema name</span></span>  <br/> |<span data-ttu-id="b2fa7-262">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b2fa7-262">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b2fa7-263">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b2fa7-263">Validation file</span></span>  <br/> |<span data-ttu-id="b2fa7-264">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b2fa7-264">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b2fa7-265">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b2fa7-265">Can be empty</span></span>  <br/> |<span data-ttu-id="b2fa7-266">False</span><span class="sxs-lookup"><span data-stu-id="b2fa7-266">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2fa7-267">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b2fa7-267">See also</span></span>



[<span data-ttu-id="b2fa7-268">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="b2fa7-268">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="b2fa7-269">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="b2fa7-269">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="b2fa7-270">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b2fa7-270">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

