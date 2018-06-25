---
title: Opération AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: L’opération AddEntityFeedback renvoie des informations d’erreur correspondant à des problèmes côté serveur.
ms.openlocfilehash: b695806f543827d78aea139ffcbd7e4af58b9fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755169"
---
# <a name="addentityfeedback-operation"></a>Opération AddEntityFeedback

L’opération **AddEntityFeedback** renvoie des informations d’erreur correspondant à des problèmes côté serveur. 
  
Cette opération s’appuie sur le type d’événement en cours de journalisation. Un des événements plus importants est **EntityAdded**, qui correspond à une entité sélectionnée. Cette opération est lot, afin qu’il peut être utilisé pour journaliser les lots d’entrées dans une demande unique. 
  
## <a name="findpeople-request-examples"></a>Exemples de requêtes FindPeople

L’opération **AddEntityFeedback** offre un moyen pour les clients journaliser les détails de l’interaction avec les entités retournées par le service. Cela peut servir comme un signal pour améliorer la pertinence dans les coulisses pour chaque client. Par exemple, les Clients peuvent utiliser cette opération pour fournir des commentaires sur les entités de personnes renvoyées à partir de **FindPeople**.
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a>Le contenu du corps demande SOAP

La demande soap contient un élément unique **EntityFeedbackEntries**. À son tour, il contient un tableau d’objets **EntityFeedbackEntry** . Chaque entrée du tableau peut contenir les éléments suivants. 
  
|**Paramètres de la demande**|**Obligatoire**|**Description**|**Type**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |Oui  <br/> |L’heure UTC l’événement s’est produite sur le côté client.  <br/> |Date/heure  <br/> |
|**ClientEventTimeLocal** <br/> |Oui  <br/> |L’heure locale de l’événement côté client.  <br/> |Date/heure  <br/> |
|**ClientId** <br/> |Oui  <br/> |Type de Client (par exemple, Outlook, OWA, etc.).  <br/> |Énumération ClientIDType  <br/> |
|**ClientSessionId** <br/> |Oui  <br/> |GUID qui identifie l’ID de session. Généré sur le client.  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |Oui  <br/> |Version du client (par exemple, 15.01.0101.000).  <br/> |String  <br/> |
|**EntityAddSource** <br/> |Non  <br/> |Source de EntityAded (par exemple, EntityRelevanceAPI, types, collés).  <br/> |Énumération EntityAddSource  <br/> |
|**EntrySequenceNumber** <br/> |Oui  <br/> |Un entier incrémenté par session client. Utilisé pour détecter la perte de données.  <br/> |Int  <br/> |
|**EventType** <br/> |Oui  <br/> |Type d’événement (par exemple, ajout de l’entité, entité supprimée).  <br/> |String  <br/> |
|**JSONPropertyBag** <br/> |Non  <br/> |Propriétés supplémentaires associées à l’événement (blob JSON de paires clé/valeur).  <br/> |Blob JSON  <br/> |
|**TargetEntityList** <br/> |Non  <br/> |Liste des entités associées à l’événement.  <br/> |Chaîne JSON  <br/> |
|**TransactionId** <br/> |Non  <br/> |ID (GUID) corrélation l’ID dans les journaux de requête.  <br/> |String  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>Réponse d’opération AddEntityFeedback réussie

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a>La réponse SOAP body contient les éléments suivants

#### <a name="errors"></a>Erreurs 
  
L’API peut se connecter à un lot d’entrées de la part de vos commentaires, nous tout ce que vous pouvez ouvrir une session. Ce champ représente le nombre d’entrées d’erreur qui ne sont pas connectés.
    
#### <a name="errordetails"></a>ErrorDetails
  
Plus d’informations concernant les erreurs ci-dessus séparant en `;`.
    
### <a name="currently-supported-values"></a>Valeurs prises en charge actuellement

|**Énumération ClientIdType**|
|:-----|
|Ordinateur de bureau  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|Messagerie  <br/> |
|MacOutlook  <br/> |
|Mobile  <br/> |
|Other  <br/> |
|Outlook  <br/> |
|OutlookService  <br/> |
|POP3  <br/> |
|Tablette  <br/> |
|Web  <br/> |
   
|**Énumération EntityAddSource**|
|:-----|
|ActiveDirectory  <br/> |
|EntityRelevanceApi  <br/> |
|EntityRelevanceApiCache  <br/> |
|ExplicitTyping  <br/> |
|LocalCache  <br/> |
|LocalCacheAndEntityRelevanceAPI  <br/> |
|Aucun  <br/> |
|Other  <br/> |
|Coller  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>Réponse d’erreur d’opération AddEntityFeedback

Pour les codes d’erreur qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>Exemple de AddEntityFeedback en association avec FindPeople

#### <a name="findpeople-request"></a>Demande FindPeople
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a>Réponse FindPeople

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a>Demande AddEntityFeedback

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> ID ID de transaction de réponse en tant que la transaction de demande AddEntityFeedback à l’aide de FindPeople d'. 
  
#### <a name="addentityfeedback-response"></a>Réponse AddEntityFeedback

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


