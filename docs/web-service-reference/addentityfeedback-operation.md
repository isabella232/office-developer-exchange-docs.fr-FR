---
title: Opération AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: L’opération AddEntityFeedback renvoie les informations d’erreur correspondant aux problèmes côté serveur.
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458438"
---
# <a name="addentityfeedback-operation"></a>Opération AddEntityFeedback

L’opération **AddEntityFeedback** renvoie les informations d’erreur correspondant aux problèmes côté serveur. 
  
Cette opération repose sur le type d’événement enregistré. L’un des événements les plus importants est **EntityAdded**, ce qui correspond à une entité sélectionnée. Cette opération étant un traitement par lots, elle peut être utilisée pour enregistrer des lots d’entrées dans une demande unique. 
  
## <a name="findpeople-request-examples"></a>Exemples de requête FindPeople

L’opération **AddEntityFeedback** permet aux clients de consigner les détails de l’interaction avec les entités renvoyées par le service. Cela peut être utilisé en tant que signal pour améliorer la pertinence en arrière-plan pour chaque client. Par exemple, les clients peuvent utiliser cette opération pour envoyer des commentaires sur les entités de personnes retournées à partir de **FindPeople**.
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="the-request-soap-body-contents"></a>Contenu du corps SOAP de la demande

La demande SOAP contient un seul élément **EntityFeedbackEntries**. Il contient à son tour un tableau d’objets **EntityFeedbackEntry** . Chaque entrée du tableau peut contenir les éléments suivants. 
  
|**Paramètres de la demande**|**Obligatoire**|**Description**|**Type**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |Oui  <br/> |Heure UTC à laquelle l’événement s’est produit côté client.  <br/> |DateTime
  <br/> |
|**ClientEventTimeLocal** <br/> |Oui  <br/> |Heure locale à laquelle l’événement s’est produit côté client.  <br/> |DateTime
  <br/> |
|**Identifi** <br/> |Oui  <br/> |Type de client (par exemple, Outlook, OWA, etc.).  <br/> |ClientIDType, énumération  <br/> |
|**ClientSessionId** <br/> |Oui  <br/> |GUID identifiant l’ID de session. Généré sur le client.  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |Oui  <br/> |Version du client (par exemple, 15.01.0101.000).  <br/> |Chaîne  <br/> |
|**EntityAddSource** <br/> |Non  <br/> |Source pour EntityAded (par exemple, EntityRelevanceAPI, types, collés).  <br/> |EntityAddSource, énumération  <br/> |
|**EntrySequenceNumber** <br/> |Oui  <br/> |Entier incrémentiel par session cliente. Utilisé pour détecter la perte de données.  <br/> |Int  <br/> |
|**EventType** <br/> |Oui  <br/> |Type d’événement (par exemple, entité ajoutée, entité supprimée).  <br/> |Chaîne  <br/> |
|**JSONPropertyBag** <br/> |Non  <br/> |Propriétés supplémentaires associées à l’événement (BLOB JSON des paires clé/valeur).  <br/> |BLOB JSON  <br/> |
|**TargetEntityList** <br/> |Non  <br/> |Liste des entités associées à l’événement.  <br/> |Chaîne JSON  <br/> |
|**TransactionId** <br/> |Non  <br/> |ID (GUID) corrélation de l’ID dans les journaux de requêtes.  <br/> |Chaîne  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>Réponse de l’opération AddEntityFeedback réussie

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a>Le corps SOAP de réponse contient les éléments suivants

#### <a name="errors"></a>Erreurs 
  
L’API peut journaliser un lot d’entrées de commentaires, Nous consignerons tout ce que nous pouvons faire. Ce champ indique le nombre d’entrées d’erreur qui n’ont pas été journalisées.
    
#### <a name="errordetails"></a>ErrorDetails
  
Les détails relatifs aux erreurs ci-dessus sont séparés par `;` .
    
### <a name="currently-supported-values"></a>Valeurs actuellement prises en charge

|**ClientIdType, énumération**|
|:-----|
|Desktop  <br/> |
|Exchange  <br/> |
|CONSÉQUENT  <br/> |
|Lync  <br/> |
|MacMail  <br/> |
|MacOutlook  <br/> |
|Mobile  <br/> |
|Autres  <br/> |
|Outlook  <br/> |
|OutlookService  <br/> |
|POP3  <br/> |
|Tablet  <br/> |
|Web  <br/> |
   
|**EntityAddSource, énumération**|
|:-----|
|ActiveDirectory  <br/> |
|EntityRelevanceApi  <br/> |
|EntityRelevanceApiCache  <br/> |
|ExplicitTyping  <br/> |
|LocalCache  <br/> |
|LocalCacheAndEntityRelevanceAPI  <br/> |
|Aucun  <br/> |
|Autres  <br/> |
|Coller  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>Réponse d’erreur d’opération AddEntityFeedback

Pour les codes d’erreur qui sont génériques à EWS, voir [ResponseCode](responsecode.md).
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>Exemple de AddEntityFeedback en association avec FindPeople

#### <a name="findpeople-request"></a>Demande FindPeople
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> Utilisation de l’ID de transaction de réponse FindPeople comme ID de transaction de demande AddEntityFeedback. 
  
#### <a name="addentityfeedback-response"></a>Réponse AddEntityFeedback

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


