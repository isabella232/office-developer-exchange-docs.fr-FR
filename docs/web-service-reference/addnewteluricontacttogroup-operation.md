---
title: Opération AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Trouvez des informations sur l’utilisation de l’opération EWS AddNewTelUriContactToGroup.
ms.openlocfilehash: 91228ec627ad928d2f1837c135af24846f811b1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464944"
---
# <a name="addnewteluricontacttogroup-operation"></a>Opération AddNewTelUriContactToGroup

Trouvez des informations sur l’utilisation de l’opération EWS **AddNewTelUriContactToGroup** . 
  
L’opération **AddNewTelUriContactToGroup** ajoute un nouveau contact à un groupe en fonction du numéro de téléphone d’un contact. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a>Utilisation de l’opération AddNewTelUriContactToGroup

Une demande d’opération **AddNewTelUriContactToGroup** soumet l’URI tel d’un contact, l’URI SIP, le numéro de téléphone et le groupe auquel ajouter le contact. Une réponse d’opération **AddNewTelUriContactToGroup** crée un personnage pour le nouveau contact. Cette opération permet aux clients d’ajouter un nouveau contact même si le contact n’a pas de nom. 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a>En-têtes SOAP d’opération AddNewTelUriContactToGroup

L’opération **AddNewTelUriContactToGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a>Exemple de requête d’opération AddNewTelUriContactToGroup : ajouter un nouveau contact à un groupe

L’exemple suivant de demande d’opération **AddNewTelUriContactToGroup** indique comment créer un contact et ajouter le nouveau contact à un groupe de messagerie instantanée à l’aide des URI tel et SIP du contact. 
  
> [!NOTE]
> Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité. 
  
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
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

Le corps SOAP de la demande contient les éléments suivants :
  
- [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)
    
- [TelUriAddress](teluriaddress.md)
    
- [ImContactSipUriAddress](imcontactsipuriaddress.md)
    
- [ImTelephoneNumber](imtelephonenumber.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a>Réponse de l’opération AddNewTelUriContactToGroup réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **AddNewTelUriContactToGroup** pour créer un contact. La réponse contient l’identificateur de personnage associé au contact, le nom d’affichage du personnage, qui est, dans ce cas, basé sur le numéro de téléphone du contact et l’identificateur d’élément du contact, qui est affiché dans le cadre de l’attribution de l’identificateur source. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <t:PersonaId Id="AAQkADE686dX3s="/>
            <t:PersonaType>Person</t:PersonaType>
            <t:CreationTime>2012-10-29T23:10:13Z</t:CreationTime>
            <t:DisplayName/>
            <t:DisplayNameFirstLast>5625550100</t:DisplayNameFirstLast>
            <t:DisplayNameLastFirst>5625550100</t:DisplayNameLastFirst>
            <t:FileAs/>
            <t:FileAsId >None</t:FileAsId>
            <t:RelevanceScore >2147483647</t:RelevanceScore>
            <t:Attributions>
               <t:Attribution>
                  <t:Id>0</t:Id>
                  <t:SourceId Id="ABhHuhCAAA=" ChangeKey="EQAAABxFU"/>
                  <t:DisplayName>Lync Contacts</t:DisplayName>
                  <t:IsWritable>false</t:IsWritable>
                  <t:IsQuickContact>true</t:IsQuickContact>
                  <t:IsHidden>false</t:IsHidden>
               </t:Attribution>
            </t:Attributions>
            <t:FileAsIds>
               <t:StringAttributedValue>
                  <t:Value>None</t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:StringAttributedValue>
            </t:FileAsIds>
            <t:OtherTelephones>
               <t:PhoneNumberAttributedValue>
                  <t:Value>
                     <t:Number>5625550100</t:Number>
                     <t:Type>Other</t:Type>
                  </t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:PhoneNumberAttributedValue>
            </t:OtherTelephones>
         </Persona>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Persona](persona.md)
    
- [PersonaId](personaid.md)
    
- [PersonaType](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [FileAsId](fileasid.md)
    
- [RelevanceScore](relevancescore.md)
    
- [Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)
    
- [Attribution (PersonaAttributionType)](attribution-personaattributiontype.md)
    
- [ID (chaîne)](id-string.md)
    
- [SourceId](sourceid.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [IsWritable](iswritable.md)
    
- [IsQuickContact](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [FileAsIds](fileasids.md)
    
- [StringAttributedValue](stringattributedvalue.md)
    
- [Valeur](value.md)
    
- [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
    
- [Attribution (String)](attribution-string.md)
    
- [OtherTelephones](othertelephones.md)
    
- [PhoneNumberAttributedValue](phonenumberattributedvalue.md)
    
- [Valeur](value.md)
    
- [Number](number.md)
    
- [Type (chaîne)](type-string.md)
    
- [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
    
- [Attribution (String)](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a>Exemple de réponse d’erreur d’opération AddNewTelUriContactToGroup

L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddNewTelUriContactToGroup** lorsque l’identificateur de groupe contient une valeur correctement formée qui n’identifie pas un groupe dans la boîte aux lettres. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [AddNewTelUriContactToGroupResponse](addnewteluricontacttogroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Personnes et contacts dans EWS dans Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

