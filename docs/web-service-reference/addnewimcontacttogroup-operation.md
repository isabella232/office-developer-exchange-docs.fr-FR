---
title: Opération AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Opération de recherche plus d’informations sur la AddNewImContactToGroup EWS.
ms.openlocfilehash: f75b89dbb6e948431d56acb9baa93fe4d4a1d939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755177"
---
# <a name="addnewimcontacttogroup-operation"></a>Opération AddNewImContactToGroup

Trouvez des informations sur l’opération EWS **AddNewImContactToGroup** . 
  
L’opération **AddNewImContactToGroup** ajoute un nouveau contact à un groupe (IM) de messagerie instantanée. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-addnewimcontacttogroup-operation"></a>Utilisation de l’opération AddNewImContactToGroup

L’opération **AddNewImContactToGroup** prend les trois arguments à ajouter un nouveau contact à un groupe de messagerie instantanée suivants : 
  
- **IMAddress,** propriété - identifie l’adresse de messagerie instantanée. Cette propriété est requise. 
    
- Propriété **DisplayName** - identifie le nom du contact complet. 
    
- Propriété **GroupId** - identifie le groupe que le contact est ajouté à. 
    
Cette opération retourne le personnage du contact qui a été ajouté au groupe.
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a>En-têtes SOAP AddNewImContactToGroup opération

L’opération **AddNewImContactToGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a>Exemple de requête d’opération AddNewImContactToGroup : ajouter un nouveau contact de messagerie instantanée à un groupe

Une requête d’opération **AddNewImContactToGroup** l’exemple suivant montre comment ajouter un nouveau contact à un groupe existant de la messagerie instantanée. La valeur de la propriété **GroupId** pour que cet exemple a été retournée à partir des résultats de l' [opération AddImGroup](addimgroup-operation.md). La propriété **ExchangeStoreId** contient la valeur de la propriété **GroupId** . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:AddNewImContactToGroup>
         <m:ImAddress>tsmith@contoso.com</m:ImAddress>
         <m:DisplayName>Tony Smith</m:DisplayName>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddNewImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> La valeur **GroupId** a été raccourcie afin de préserver la lisibilité. 
  
La demande SOAP body contient les éléments suivants :
  
- [AddNewImContactToGroup](addnewimcontacttogroup.md)
    
- [ImAddress (chaîne)](imaddress-string.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a>Réponse d’opération AddNewImContactToGroup réussie

L’exemple suivant montre une réponse positive à une demande d’opération **AddNewImContactToGroup** . La réponse contient le personnage du contact nouvellement créé. Le contact est ajouté au dossier Contacts rapides dans Exchange. 
  
> [!NOTE]
> Les identificateurs ont été réduits afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
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
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Attribution>
            <Id>0</Id>
            <SourceId Id="BtF8oI7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                      ChangeKey="EQAAABYAAABtF8oIQoTbWAAAAAAyg" />
            <DisplayName>Outlook</DisplayName>
            <IsWritable>true</IsWritable>
            <IsQuickContact>true</IsQuickContact>
            <IsHidden>false</IsHidden>
            <FolderId Id="AAMkAGQ1MjJjMTBkLTc4YhQoTbWAAAAAAvZAAA=" 
                      ChangeKey="AQAAAA==" />
          </Attribution>
        </Attributions>
        <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddressAttributedValue>
            <Value>
              <Name>Tony Smith</Name>
              <Address>tsmith@contoso.com</Address>
              <RoutingType>SMTP</RoutingType>
            </Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </EmailAddressAttributedValue>
        </Emails1>
        <ImAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>tsmith@contoso.com</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </ImAddresses>
      </Persona>
    </AddNewImContactToGroupResponse>
  </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md)
    
- [Personnage](persona.md)
    
- [PersonaId](personaid.md)
    
- [PersonaType](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAsId](fileasid.md)
    
- [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
    
- [Nom (EmailAddressType)](name-emailaddresstype.md)
    
- [Adresse (chaîne)](address-string.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [ImAddress (chaîne)](imaddress-string.md)
    
- [RelevanceScore](relevancescore.md)
    
- [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)
    
- [Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
    
- [ID (chaîne)](id-string.md)
    
- [ID source](sourceid.md)
    
- [IsWritable](iswritable.md)
    
- [IsQuickContact](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [FolderId](folderid.md)
    
- [DisplayNames](displaynames.md)
    
- [StringAttributedValue](stringattributedvalue.md)
    
- [Valeur (ArrayOfStringValueType)](value-arrayofstringvaluetype.md)
    
- [FileAsIds](fileasids.md)
    
- [Emails1](emails1.md)
    
- [EmailAddressAttributedValue](emailaddressattributedvalue.md)
    
- [ImAddresses](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a>Réponse d’erreur d’opération AddNewImContactToGroup

L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddNewImContactToGroup** . Il s’agit d’une réponse à une demande pour ajouter un contact à un groupe qui ne figure pas dans la boîte aux lettres du demandeur. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [AddNewImContactToGroupResponse](addnewimcontacttogroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [MessageXml](messagexml.md)
    
Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi



[Opération AddImGroup](addimgroup-operation.md)
  
[Opération AddImContactToGroup](addimcontacttogroup-operation.md)
  
[Opération AddImGroup](addimgroup-operation.md)
  
[Opération RemoveImGroup](removeimgroup-operation.md)
  
[Opération SetImGroup](setimgroup-operation.md)


[Personnes et contacts dans EWS dans Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

