---
title: Opération GetImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: Opération de recherche plus d’informations sur la GetImItemList EWS.
ms.openlocfilehash: 3977b0ad31e819cd973ce261ba3152b3840003b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756642"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="92ec4-103">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="92ec4-103">GetImItemList operation</span></span>

<span data-ttu-id="92ec4-104">Trouvez des informations sur l’opération EWS **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="92ec4-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="92ec4-105">Utilisation de l’opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="92ec4-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="92ec4-106">L’opération **GetImItemList** récupère la liste des groupes de la messagerie instantanée et de contact de messagerie instantanée personnages dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="92ec4-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="92ec4-107">L’opération **GetImItemList** ne prend aucun argument.</span><span class="sxs-lookup"><span data-stu-id="92ec4-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="92ec4-108">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="92ec4-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="92ec4-109">En-têtes SOAP GetImItemList opération</span><span class="sxs-lookup"><span data-stu-id="92ec4-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="92ec4-110">L’opération **GetImItemList** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="92ec4-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="92ec4-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="92ec4-111">**Header name**</span></span>|<span data-ttu-id="92ec4-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92ec4-112">**Element**</span></span>|<span data-ttu-id="92ec4-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="92ec4-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="92ec4-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="92ec4-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="92ec4-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="92ec4-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="92ec4-116">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="92ec4-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="92ec4-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92ec4-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92ec4-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="92ec4-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="92ec4-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="92ec4-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="92ec4-120">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="92ec4-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="92ec4-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92ec4-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92ec4-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="92ec4-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="92ec4-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="92ec4-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="92ec4-124">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="92ec4-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="92ec4-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92ec4-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92ec4-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="92ec4-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="92ec4-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="92ec4-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="92ec4-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="92ec4-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="92ec4-129">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="92ec4-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="92ec4-130">Exemple de requête d’opération GetImItemList : demande de votre liste de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="92ec4-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="92ec4-131">Une demande d’opération **GetImItemList** l’exemple suivant montre comment demander la liste des groupes de messagerie instantanée et de contact de messagerie instantanée personnages dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="92ec4-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="92ec4-132">L’élément **GetImItemList** est le seul élément dans le corps SOAP.</span><span class="sxs-lookup"><span data-stu-id="92ec4-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="92ec4-133">La demande SOAP body contienne l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="92ec4-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="92ec4-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="92ec4-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="92ec4-135">Réponse d’opération GetImItemList réussie</span><span class="sxs-lookup"><span data-stu-id="92ec4-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="92ec4-136">L’exemple suivant montre une réponse positive à une demande d’opération **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="92ec4-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="92ec4-137">La réponse contient quatre groupes de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="92ec4-137">The response contains four IM groups.</span></span> <span data-ttu-id="92ec4-138">Trois des groupes de messagerie instantanée, autres Contacts, balisée et Favoris — sont des groupes par défaut dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="92ec4-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="92ec4-139">Le groupe MyCustomGroup2 est un groupe personnalisé créé par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="92ec4-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="92ec4-140">Les groupes autres Contacts et balisée n’ont pas de membres.</span><span class="sxs-lookup"><span data-stu-id="92ec4-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="92ec4-141">Le groupe de favoris a un seul membre de contact.</span><span class="sxs-lookup"><span data-stu-id="92ec4-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="92ec4-142">Le MyCustomGroup2 a deux contacts membre.</span><span class="sxs-lookup"><span data-stu-id="92ec4-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="92ec4-143">Les identificateurs d’élément sont fournies afin que les demandes **GetItem** suivantes peuvent être effectuées pour obtenir plus d’informations sur les contacts de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="92ec4-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="92ec4-144">Cet exemple renvoie les deux personnes.</span><span class="sxs-lookup"><span data-stu-id="92ec4-144">This example returns two personas.</span></span> <span data-ttu-id="92ec4-145">Le premier personnage représente deux éléments de contact : Anthony Smith et Tony Smith.</span><span class="sxs-lookup"><span data-stu-id="92ec4-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="92ec4-146">Les informations de contact combinées sont renvoyées dans l’objet **personnage** .</span><span class="sxs-lookup"><span data-stu-id="92ec4-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="92ec4-147">Le deuxième personnage représente un seul contact dont le nom complet de Terence Adams.</span><span class="sxs-lookup"><span data-stu-id="92ec4-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="92ec4-148">Les identificateurs de magasin Exchange, identificateurs d’éléments, identificateurs source, les identificateurs de dossier et identificateurs personnage ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="92ec4-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="92ec4-149">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="92ec4-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92ec4-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="92ec4-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="92ec4-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92ec4-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92ec4-152">ImItemList</span><span class="sxs-lookup"><span data-stu-id="92ec4-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="92ec4-153">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="92ec4-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="92ec4-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="92ec4-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="92ec4-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="92ec4-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="92ec4-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="92ec4-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="92ec4-157">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="92ec4-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="92ec4-158">Personnages</span><span class="sxs-lookup"><span data-stu-id="92ec4-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="92ec4-159">PersonaId</span><span class="sxs-lookup"><span data-stu-id="92ec4-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="92ec4-160">PersonaType</span><span class="sxs-lookup"><span data-stu-id="92ec4-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="92ec4-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="92ec4-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="92ec4-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="92ec4-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="92ec4-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="92ec4-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="92ec4-164">Classer sous</span><span class="sxs-lookup"><span data-stu-id="92ec4-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="92ec4-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="92ec4-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="92ec4-166">Prénom</span><span class="sxs-lookup"><span data-stu-id="92ec4-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="92ec4-167">Surname</span><span class="sxs-lookup"><span data-stu-id="92ec4-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="92ec4-168">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="92ec4-169">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="92ec4-170">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="92ec4-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="92ec4-172">ImAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="92ec4-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="92ec4-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="92ec4-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="92ec4-174">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="92ec4-175">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="92ec4-176">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="92ec4-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="92ec4-177">ID source</span><span class="sxs-lookup"><span data-stu-id="92ec4-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="92ec4-178">IsWritable</span><span class="sxs-lookup"><span data-stu-id="92ec4-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="92ec4-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="92ec4-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="92ec4-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="92ec4-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="92ec4-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="92ec4-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="92ec4-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="92ec4-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="92ec4-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="92ec4-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="92ec4-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="92ec4-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="92ec4-185">GivenNames</span><span class="sxs-lookup"><span data-stu-id="92ec4-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="92ec4-186">Prénoms</span><span class="sxs-lookup"><span data-stu-id="92ec4-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="92ec4-187">HomePhones</span><span class="sxs-lookup"><span data-stu-id="92ec4-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="92ec4-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="92ec4-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="92ec4-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="92ec4-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="92ec4-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="92ec4-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="92ec4-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="92ec4-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="92ec4-192">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="92ec4-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="92ec4-193">Valeur (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="92ec4-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="92ec4-194">Réponse d’erreur d’opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="92ec4-194">GetImItemList operation error response</span></span>

<span data-ttu-id="92ec4-195">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetImItemList** .</span><span class="sxs-lookup"><span data-stu-id="92ec4-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="92ec4-196">Il s’agit d’une réponse à une demande qui contient une version serveur demandé incorrect dans l’en-tête SOAP.</span><span class="sxs-lookup"><span data-stu-id="92ec4-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="92ec4-197">Cette réponse d’erreur est une erreur SOAP et n’est pas représentée dans le schéma EWS.</span><span class="sxs-lookup"><span data-stu-id="92ec4-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="92ec4-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="92ec4-198">See also</span></span>

- [<span data-ttu-id="92ec4-199">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="92ec4-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="92ec4-200">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="92ec4-200">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="92ec4-201">Opération GetImItems</span><span class="sxs-lookup"><span data-stu-id="92ec4-201">GetImItems operation</span></span>](getimitems-operation.md)
    

