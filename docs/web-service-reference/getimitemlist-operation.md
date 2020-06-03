---
title: Opération GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: Trouvez des informations sur l’opération EWS GetImItemList.
ms.openlocfilehash: aabe84054b93e7de8af6145942493a0224932e45
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456065"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="46385-103">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="46385-103">GetImItemList operation</span></span>

<span data-ttu-id="46385-104">Trouvez des informations sur l’opération EWS **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="46385-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="46385-105">Utilisation de l’opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="46385-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="46385-106">L’opération **GetImItemList** récupère la liste des groupes de messagerie instantanée et des personnes de contact de messagerie instantanée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="46385-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="46385-107">L’opération **GetImItemList** ne prend aucun argument.</span><span class="sxs-lookup"><span data-stu-id="46385-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="46385-108">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="46385-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="46385-109">En-têtes SOAP d’opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="46385-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="46385-110">L’opération **GetImItemList** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="46385-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="46385-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="46385-111">**Header name**</span></span>|<span data-ttu-id="46385-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="46385-112">**Element**</span></span>|<span data-ttu-id="46385-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="46385-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="46385-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="46385-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="46385-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="46385-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="46385-116">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="46385-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="46385-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="46385-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="46385-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="46385-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="46385-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="46385-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="46385-120">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="46385-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="46385-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="46385-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="46385-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="46385-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="46385-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="46385-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="46385-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="46385-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="46385-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="46385-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="46385-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="46385-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="46385-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="46385-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="46385-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="46385-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="46385-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="46385-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="46385-130">Exemple de requête d’opération GetImItemList : demander votre liste d’éléments de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="46385-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="46385-131">L’exemple suivant de demande d’opération **GetImItemList** montre comment demander la liste des personnages de groupes de messagerie instantanée et de contacts de messagerie instantanée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="46385-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="46385-132">L’élément **GetImItemList** est l’unique option de l’élément dans le corps SOAP.</span><span class="sxs-lookup"><span data-stu-id="46385-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
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
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="46385-133">Le corps SOAP de la demande contient l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="46385-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="46385-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="46385-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="46385-135">Réponse de l’opération GetImItemList réussie</span><span class="sxs-lookup"><span data-stu-id="46385-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="46385-136">L’exemple suivant montre une réponse réussie à une demande d’opération **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="46385-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="46385-137">La réponse contient quatre groupes de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="46385-137">The response contains four IM groups.</span></span> <span data-ttu-id="46385-138">Trois des groupes de messagerie instantanée (autres contacts, balises et favoris) sont des groupes par défaut dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="46385-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="46385-139">Le groupe MyCustomGroup2 est un groupe personnalisé créé par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="46385-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="46385-140">Les autres contacts et les groupes balisés n’ont pas de membres.</span><span class="sxs-lookup"><span data-stu-id="46385-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="46385-141">Le groupe favoris a un seul membre de contact.</span><span class="sxs-lookup"><span data-stu-id="46385-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="46385-142">Le MyCustomGroup2 a deux contacts membres.</span><span class="sxs-lookup"><span data-stu-id="46385-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="46385-143">Les identificateurs d’élément sont fournis de sorte que les demandes **GetItem** suivantes puissent être effectuées pour obtenir plus d’informations sur les contacts de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="46385-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="46385-144">Cet exemple montre comment renvoyer deux personnages.</span><span class="sxs-lookup"><span data-stu-id="46385-144">This example returns two personas.</span></span> <span data-ttu-id="46385-145">Le premier personnage représente deux contacts : Anthony Smith et Tony Smith.</span><span class="sxs-lookup"><span data-stu-id="46385-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="46385-146">Les informations de contact combinées sont renvoyées dans l’objet **Persona** .</span><span class="sxs-lookup"><span data-stu-id="46385-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="46385-147">Le deuxième personnage représente un contact unique portant le nom d’affichage Terence Adams.</span><span class="sxs-lookup"><span data-stu-id="46385-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="46385-148">Les identificateurs de banque Exchange, les identificateurs d’élément, les identificateurs source, les identificateurs de dossier et les identificateurs de personnages ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="46385-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Other Contacts</DisplayName>
                  <GroupType>IPM.DistList.MOC.OtherContacts</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLThQoTbWAAAAAAQUAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Tagged</DisplayName>
                  <GroupType>IPM.DistList.MOC.Tagged</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJAAQTAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Favorites</DisplayName>
                  <GroupType>IPM.DistList.MOC.Favorites</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTAAAAAQSAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1MjJtt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
               <ImGroup>
                  <DisplayName>MyCustomGroup2</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjKAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1Matt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                     <ItemId Id="AAMkAGQ1MjJjMTBkTbWAAAAAAveAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
            </Groups>
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4YkZmRkYQAQAFgxE1nBcqRGgYWWorM9/+s=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-12T22:14:36Z</CreationTime>
                  <DisplayName>Anthony Smith</DisplayName>
                  <DisplayNameFirstLast>Anthony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Smith Anthony</DisplayNameLastFirst>
                  <FileAs>Smith, Anthony</FileAs>
                  <FileAsId>LastCommaFirst</FileAsId>
                  <GivenName>Anthony</GivenName>
                  <Surname>Smith</Surname>
                  <EmailAddress>
                     <Name>tsmith@contoso.com</Name>
                     <EmailAddress>tsmith@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>tsmith@contoso.com</Name>
                        <EmailAddress>tsmith@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AQMkAGQ1MjIAYzEwZC03OGNlLTQ5Bq239uFChNtYAAAIvDAAAAA==" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAADB3" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>false</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AQMkAGQ1MjIAYzEMikE3AQBtF8oI7iVOQatt/bhQoTbWAAADEAAAAA==" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                     <Attribution>
                        <Id>1</Id>
                        <SourceId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04/bhQoTbWAAAAAAveAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAym" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Qatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Anthony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAses>
                     <StringAttributedValue>
                        <Value>Smith, Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAses>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>LastCommaFirst</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <GivenNames>
                     <StringAttributedValue>
                        <Value>Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </GivenNames>
                  <Surnames>
                     <StringAttributedValue>
                        <Value>Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </Surnames>
                  <HomePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550110</Number>
                           <Type>Home</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </HomePhones>
                  <MobilePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550120</Number>
                           <Type>Mobile</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </MobilePhones>
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>tsmith@contoso.com</Name>
                           <EmailAddress>tsmith@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLkYQAQAJ3EkhEEXN5KufGbSYJanZk=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-05T23:06:58Z</CreationTime>
                  <DisplayName>Terence Adams</DisplayName>
                  <DisplayNameFirstLast>Terence Adams</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Terence Adams</DisplayNameLastFirst>
                  <FileAsId>None</FileAsId>
                  <EmailAddress>
                     <Name>Terence Adams</Name>
                     <EmailAddress>tadams@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>Terence Adams</Name>
                        <EmailAddress>tadams@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tadams@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkAGQ1MjVOQatt/bhQoTbWAAAA7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAyg" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2rBtF8oI7iVOQatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Terence Adams</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>Terence Adams</Name>
                           <EmailAddress>tadams@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tadams@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="46385-149">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="46385-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="46385-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="46385-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="46385-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="46385-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="46385-152">ImItemList</span><span class="sxs-lookup"><span data-stu-id="46385-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="46385-153">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="46385-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="46385-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="46385-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="46385-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="46385-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="46385-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="46385-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="46385-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="46385-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="46385-158">Personnages</span><span class="sxs-lookup"><span data-stu-id="46385-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="46385-159">PersonaId</span><span class="sxs-lookup"><span data-stu-id="46385-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="46385-160">PersonaType</span><span class="sxs-lookup"><span data-stu-id="46385-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="46385-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="46385-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="46385-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="46385-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="46385-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="46385-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="46385-164">FileAs</span><span class="sxs-lookup"><span data-stu-id="46385-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="46385-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="46385-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="46385-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="46385-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="46385-167">Surname</span><span class="sxs-lookup"><span data-stu-id="46385-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="46385-168">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="46385-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="46385-169">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="46385-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="46385-170">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="46385-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="46385-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="46385-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="46385-172">IMAddress (String)</span><span class="sxs-lookup"><span data-stu-id="46385-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="46385-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="46385-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="46385-174">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="46385-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="46385-175">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="46385-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="46385-176">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="46385-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="46385-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="46385-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="46385-178">IsWritable</span><span class="sxs-lookup"><span data-stu-id="46385-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="46385-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="46385-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="46385-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="46385-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="46385-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="46385-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="46385-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="46385-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="46385-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="46385-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="46385-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="46385-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="46385-185">GivenNames</span><span class="sxs-lookup"><span data-stu-id="46385-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="46385-186">Nom</span><span class="sxs-lookup"><span data-stu-id="46385-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="46385-187">HomePhones</span><span class="sxs-lookup"><span data-stu-id="46385-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="46385-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="46385-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="46385-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="46385-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="46385-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="46385-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="46385-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="46385-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="46385-192">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="46385-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="46385-193">Valeur (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="46385-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="46385-194">Réponse d’erreur d’opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="46385-194">GetImItemList operation error response</span></span>

<span data-ttu-id="46385-195">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="46385-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="46385-196">Il s’agit d’une réponse à une demande contenant une version de serveur demandée incorrecte dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="46385-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="46385-197">Cette réponse d’erreur est une erreur SOAP et n’est pas représentée dans le schéma EWS.</span><span class="sxs-lookup"><span data-stu-id="46385-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="46385-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="46385-198">See also</span></span>

- [<span data-ttu-id="46385-199">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="46385-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="46385-200">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="46385-200">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="46385-201">Opération GetImItems</span><span class="sxs-lookup"><span data-stu-id="46385-201">GetImItems operation</span></span>](getimitems-operation.md)
    

