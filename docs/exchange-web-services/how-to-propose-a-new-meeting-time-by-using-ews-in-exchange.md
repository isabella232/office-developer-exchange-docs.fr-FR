---
title: Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Découvrez comment proposer de nouvelles heures de réunion à partir de votre application Exchange client à l’aide d’EWS dans Exchange.
ms.openlocfilehash: a6406aaef2005e74165e647510af891d2a59503e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522228"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange

Découvrez comment proposer de nouvelles heures de réunion à partir de votre application Exchange client à l’aide d’EWS dans Exchange.
  
La fonctionnalité proposer une nouvelle heure permet aux participants de proposer de nouvelles heures de réunion à l’organisateur de la réunion dans le cadre du flux de travail Exchange calendrier. Lorsqu’un participant propose une nouvelle réunion, l’organisateur peut utiliser la nouvelle heure de réunion proposée pour mettre à jour la réunion et envoyer des mises à jour à tous les participants. Avant de permettre aux participants de proposer de nouvelles heures de réunion, vous devez déterminer si l’organisateur autorise les propositions de nouvelles heures. Cet article explique comment déterminer si vous pouvez proposer une nouvelle heure et comment utiliser EWS pour proposer une nouvelle heure.
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Déterminer si vous pouvez proposer une nouvelle heure pour une réunion à l’aide d’EWS
<a name="bk_Determine"> </a>

Avant de pouvoir proposer une nouvelle heure pour une réunion, vous devez trouver une référence à cette réunion et déterminer si l’organisateur de la réunion a configuré la réunion pour prendre en charge les nouvelles propositions d’heure. Vous pouvez obtenir une référence à une réunion en faisant l’une des choses suivantes : 
  
- Recherche de la demande de réunion dans la boîte de réception
    
- Recherche du rendez-vous dans le calendrier
    
Pour rechercher une référence de réunion, utilisez les étapes suivantes :
  
1. Utilisez [l’opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS (ou la méthode d’API gérée EWS [Folder.FindItems)](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) pour rechercher la demande de réunion cible ou l’élément de calendrier. Vous pouvez également utiliser l’opération [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS pour obtenir l’identificateur de la demande de réunion cible ou de l’élément de calendrier. 
    
2. Parse the results of the **FindItem** operation (or **Folder.FindItems** method) to get the item identifier of the meeting item. 
    
3. Utilisez [l’opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS pour obtenir les objets de réponse pour la réunion. 
    
Le XML suivant indique ce qui est envoyé pour demander les objets de réponse sur un élément.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

La réponse de l’opération **GetItem** ressemblera au code XML suivant si vous demandez l’identificateur de l’élément, l’heure de début et de fin de la réunion, la collection d’objets de réponse et si l’organisateur autorise les modifications proposées à l’heure de la réunion. La collection d’objets response, représentée par l’élément [ResponseObjects,](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) contient l’ensemble de réponses valides pour l’élément de calendrier. **L’élément ProposeNewTime** est un objet de réponse qui indique que l’utilisateur peut proposer une nouvelle heure pour la réunion. Les [éléments AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)et [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) représentent les objets de réponse que vous pouvez utiliser pour proposer une nouvelle heure de réunion à l’organisateur de la réunion. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a>Proposer une nouvelle heure de réunion à l’aide d’EWS
<a name="bk_Propose"> </a>

Si vous avez reçu un objet de réponse **ProposeNewTime** lorsque vous avez utilisé l’opération **GetItem** pour obtenir un élément de calendrier ou une demande de réunion, vous pouvez répondre avec une nouvelle heure de réunion proposée. Si vous n’avez pas reçu d’objet de réponse **ProposeNewTime,** vous ne pourrez pas proposer une nouvelle heure de réunion dans le cadre du flux de travail de calendrier. Vous pouvez toutefois répondre à l’organisateur pour demander une nouvelle heure de réunion. Si vous recevez un objet de réponse **ProposeNewTime,** vous pouvez répondre à la réunion en référentant son identificateur et proposer une nouvelle heure de réunion à l’organisateur. C’est là que **l’objet** de réponse ProposeNewTime est différent du modèle d’objet de réponse classique dans la façon dont vous ne répondez pas avec un objet de réponse **ProposeNewTime.** Vous utilisez l’un des autres objets de réponse à la réunion, tels que **AcceptItem,** **TentativelyAcceptItem** ou **DeclineItem,** pour proposer une nouvelle réunion. Cet exemple utilise **l’objet de réponse AcceptItem.** 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

La réponse à cette demande contient l’identificateur de l’élément de calendrier qui a été ajouté au calendrier du participant et une copie de la demande de réunion qui a été placée dans le dossier Éléments supprimés du participant. Le message de réponse avec la nouvelle proposition d’heure a également été enregistré dans le dossier Éléments envoyés du participant (vous devez trouver le message de réponse à la réunion pour obtenir un handle dessus).
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

L’organisateur reçoit un message [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) lorsque le participant répond avec une nouvelle heure de réunion proposée. Le message **MeetingResponse** contient les nouvelles heures de début et de fin de réunion proposées, ainsi que l’identificateur de l’élément de calendrier associé dans le calendrier de l’organisateur. L’organisateur peut utiliser ces informations pour mettre à jour son élément de calendrier existant pour la réunion. Voici le flux de travail pour que l’organisateur réponde à un message **MeetingResponse** qui propose une nouvelle heure de réunion : 
  
1. Déterminez si **les éléments ProposedStart** ou **ProposedEnd** ont été définies dans **MeetingResponse**. Si c’est le cas, allez à l’étape 2. Si ce n’est pas le cas, le message **MeetingResponse** indique uniquement si le participant a accepté, provisoirement accepté ou refusé la réunion. 
    
2. Obtenez l’élément de calendrier existant de l’organisateur pour la réunion à l’aide de l’identificateur EWS renvoyé dans l’élément **AssociatedCalendarItemId.** 
    
3. Comparez l’heure de début et de fin d’origine à la nouvelle heure de réunion proposée. Si la nouvelle heure de réunion proposée est acceptable pour l’organisateur, allez à l’étape 4. Dans le cas contraire, l’organisateur de la réunion peut ignorer l’heure de réunion proposée ou envoyer une réponse par courrier électronique au participant qui a proposé la nouvelle heure de réunion.
    
4. (Facultatif) Effectuez un appel d’opération [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS pour déterminer si l’heure proposée fonctionne pour tous les participants, y compris les boîtes aux lettres de salle et de ressources. (Vous pouvez également utiliser la méthode d’API gérée EWS [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) pour ce faire.) 
    
5. L’organisateur peut ensuite mettre à jour sa réunion avec les nouvelles heures de réunion proposées et envoyer les mises à jour à tous les participants à l’aide de l’opération [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS (ou de la méthode d’API gérée EWS [Appointment.Update).](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) 
    
La figure suivante illustre le processus qui se produit entre l’organisateur de la réunion, le participant et le serveur Exchange qui a géré les appels EWS.
  
**Figure 1. Processus de proposition d’une nouvelle heure de réunion**

![La figure illustre le flux de travail entre l’organisateur, Exchange et un participant lorsqu’un nouvel horaire de réunion est proposé. Si l’organisateur autorise de nouvelles propositions de réunion, un participant peut proposer un nouvel horaire de réunion avec un objet de réponse.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Différences entre les versions
<a name="bk_Behavior"> </a>

La fonctionnalité proposer une nouvelle heure a été introduite dans Exchange version de build 15.00.0800.007. Dans les versions antérieures de Exchange, les utilisateurs de l’application EWS doivent envoyer un e-mail distinct à l’organisateur de la réunion pour demander une autre heure de réunion. 
  
## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

