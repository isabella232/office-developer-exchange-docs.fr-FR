---
title: FreeBusyViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyViewOptions
api_type:
- schema
ms.assetid: c07f3ddb-874b-4d30-a60e-7e5c7793bb6f
description: L’élément FreeBusyViewOptions spécifie le type d’informations de libre/occupé renvoyées dans la réponse.
ms.openlocfilehash: fc9b3e32dff5ae984d2921a3a46319a6f3e89da8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526220"
---
# <a name="freebusyviewoptions"></a>FreeBusyViewOptions

**L’élément FreeBusyViewOptions** spécifie le type d’informations de libre/occupé renvoyées dans la réponse. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 **FreeBusyViewOptionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |Identifie l’étendue de temps à interroger pour les informations de disponibilité de l’utilisateur.  <br/> |
|[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) <br/> |Représente la différence de temps entre deux emplacements successifs dans la **vue FreeBusyMerged.**  <br/> |
|[RequestedView](requestedview.md) <br/> |Définit le type d’informations de calendrier qu’un client demande.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur. Il s’agit d’un élément racine.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et ne peut se produire qu’une seule fois s’il est utilisé. Cette valeur peut être null si la valeur de l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) n’est pas null. 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire /genre/ de l’ordinateur qui exécute Microsoft® Exchange Server 2007 où le rôle serveur d’accès au client est installé. 
  
## <a name="example"></a>Exemple

L’exemple suivant obtient une liste de réunions et un flux de libre/occupé par intervalles de 60 minutes.
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </TimeZone>
      <MailboxDataArray>
        <MailboxData xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@ExServer.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

