---
title: Opération AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Trouvez des informations sur l’opération EWS AddImGroup.
ms.openlocfilehash: 38ed12a741d46fe998dc0079ed13973ce9edf5ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462814"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="f1ce7-103">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-103">AddImGroup operation</span></span>

<span data-ttu-id="f1ce7-104">Trouvez des informations sur l’opération EWS **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="f1ce7-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="f1ce7-105">L’opération **AddImGroup** les services Web Exchange (EWS) ajoute un nouveau groupe de messagerie instantanée à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="f1ce7-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="f1ce7-107">Utilisation de l’opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="f1ce7-108">L’opération **AddImGroup** ne prend qu’un seul argument Nom complet.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="f1ce7-109">Cette opération renvoie le nom complet, le type de groupe et l’identificateur de la Banque d’Exchange du nouveau groupe.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="f1ce7-110">L’opération **AddImGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="f1ce7-111">**Tableau 1. En-têtes SOAP d’opération AddImGroup**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="f1ce7-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-112">**Header name**</span></span>|<span data-ttu-id="f1ce7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-113">**Element**</span></span>|<span data-ttu-id="f1ce7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f1ce7-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="f1ce7-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f1ce7-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="f1ce7-117">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="f1ce7-118">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f1ce7-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="f1ce7-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="f1ce7-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="f1ce7-121">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="f1ce7-122">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f1ce7-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="f1ce7-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f1ce7-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f1ce7-125">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="f1ce7-126">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f1ce7-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="f1ce7-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="f1ce7-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f1ce7-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f1ce7-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="f1ce7-130">Ceci s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="f1ce7-131">Exemple de requête d’opération AddImGroup : créer un groupe de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="f1ce7-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="f1ce7-132">L’exemple suivant de demande d’opération **AddImGroup** montre comment créer un groupe de messagerie instantanée nommé MyCustomerGroup.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f1ce7-133">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="f1ce7-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f1ce7-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="f1ce7-135">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="f1ce7-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="f1ce7-136">Réponse de l’opération AddImGroup réussie</span><span class="sxs-lookup"><span data-stu-id="f1ce7-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="f1ce7-137">L’exemple suivant montre une réponse réussie à une demande d’opération **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="f1ce7-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="f1ce7-138">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="f1ce7-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f1ce7-139">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="f1ce7-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="f1ce7-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f1ce7-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f1ce7-141">Imgroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="f1ce7-142">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="f1ce7-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="f1ce7-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="f1ce7-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="f1ce7-144">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="f1ce7-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="f1ce7-145">Réponse d’erreur d’opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-145">AddImGroup operation error response</span></span>

<span data-ttu-id="f1ce7-146">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="f1ce7-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="f1ce7-147">Il s’agit d’une réponse à une requête qui contient un caractère qui ne peut pas être utilisé dans un nom d’affichage.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="f1ce7-148">Notez qu’il s’agit d’une erreur SOAP et non d’un message d’erreur basé sur un schéma.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="f1ce7-149">Le nom complet soumis dans la demande est ~ ! @ # $% ^ &amp; , et l’erreur se produit sur le &amp; caractère.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="f1ce7-150">Le &amp; caractère s’est produit sur la onzième ligne et le caractère 33e dans la charge utile de la demande.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="f1ce7-151">La réponse a été renvoyée avec un code HTTP 500.</span><span class="sxs-lookup"><span data-stu-id="f1ce7-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f1ce7-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1ce7-152">See also</span></span>

- [<span data-ttu-id="f1ce7-153">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f1ce7-153">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="f1ce7-154">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="f1ce7-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="f1ce7-155">SetImGroup</span></span>](setimgroup.md)
    

