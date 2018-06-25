---
title: Opération AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Opération de recherche plus d’informations sur la AddDistributionGroupToImList EWS.
ms.openlocfilehash: 7c562c317890a4cffb9e5844ea41c1096a8595b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755161"
---
# <a name="adddistributiongrouptoimlist-operation"></a>Opération AddDistributionGroupToImList

Trouvez des informations sur l’opération EWS **AddDistributionGroupToImList** . 
  
L’opération d’Exchange Web Services (EWS) **AddDistributionGroupToImList** ajoute un groupe de distribution à la liste (IM) dans le magasin de contacts unifié de messagerie instantanée. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a>Utilisation de l’opération AddDistributionGroupToImList

L’opération **AddDistributionGroupToImList** prend un argument unique qui identifie un groupe de distribution à ajouter à la liste de messagerie instantanée. Cette opération ne crée pas d’un groupe de distribution ; le groupe de distribution doit déjà être créé. 
  
Cette opération peut utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.
  
**Le tableau 1. En-têtes SOAP AddDistributionGroupToImList opération**

|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Ceci s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Ceci s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Ceci s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cela s’applique à une réponse.  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a>Exemple de requête d’opération AddDistributionGroupToImList

Une requête d’opération **AddDistributionGroupToImList** l’exemple suivant montre comment ajouter un groupe de distribution à la liste de messagerie instantanée. 
  
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
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

La demande SOAP body contient les éléments suivants :
  
- [AddDistributionGroupToImList](adddistributiongrouptoimlist.md)   
- [SmtpAddress](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a>Réponse d’opération AddDistributionGroupToImList réussie

L’exemple suivant montre une réponse positive à une demande d’opération **AddDistributionGroupToImList** . 
  
La réponse correcte contient le nom complet du groupe distribution, la classe de la banque Exchange pour le groupe de distribution et l’identificateur EWS du nouveau groupe de distribution.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [ImGroup](imgroup.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a>Opération AddDistributionGroupToImList ErrorInvalidImDistributionGroupSmtpAddress réponse d’erreur

L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddDistributionGroupToImList** . La réponse d’erreur se produit lorsqu’une tentative est effectuée pour ajouter un groupe de distribution qui n’existe pas dans la banque d’informations Exchange. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [AddDistributionGroupToImListResponse](adddistributiongrouptoimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Personnes et contacts dans EWS dans Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [AddImGroup](addimgroup-operation.md)   
- [RemoveImGroup](removeimgroup-operation.md)
    

