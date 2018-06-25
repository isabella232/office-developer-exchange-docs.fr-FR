---
title: Proposer une nouvelle heure de réunion à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Découvrez comment proposer de nouvelles dates de réunion à partir de votre application de client Exchange à l’aide de EWS dans Exchange.
ms.openlocfilehash: f9edd8511332474a728635a6aa369a772da24786
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754923"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a>Proposer une nouvelle heure de réunion à l’aide de EWS dans Exchange

Découvrez comment proposer de nouvelles dates de réunion à partir de votre application de client Exchange à l’aide de EWS dans Exchange.
  
La fonctionnalité de temps de nouveau proposer permet aux participants de proposer de nouvelles dates de réunion à l’organisateur de la réunion dans le cadre du flux de travail calendrier Exchange. Lorsqu’un participant propose une nouvelle réunion, l’organisateur peut utiliser la nouvelle heure de réunion pour mettre à jour de la réunion et envoyer des mises à jour à tous les participants. Avant de pouvoir activer aux participants de proposer de nouvelles dates de réunion, vous devez déterminer si l’organisateur autorise de nouvelles propositions d’horaires. Cet article explique comment déterminer si vous pouvez proposer une nouvelle heure et comment utiliser EWS pour proposer une nouvelle heure.
  
> [!NOTE]
> L’API managée EWS n’implémente pas cette fonctionnalité. 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a>Déterminer si vous pouvez proposer une nouvelle heure pour une réunion à l’aide de EWS
<a name="bk_Determine"> </a>

Avant de pouvoir proposer une nouvelle heure pour une réunion, vous devez trouver une référence à cette réunion et de déterminer si l’organisateur de la réunion configuré la réunion à prendre en charge de nouvelles propositions d’horaires. Vous pouvez obtenir une référence à une réunion en effectuant une des options suivantes : 
  
- Recherche de la demande de réunion dans la boîte de réception
    
- Recherche de rendez-vous dans le calendrier
    
Pour rechercher une référence de la réunion, procédez comme suit :
  
1. Utilisez l’opération EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou la méthode d’API managées [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) ) pour trouver la cible élément de calendrier ou de demande de réunion. Sinon, vous pouvez utiliser l’opération EWS [SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) pour obtenir l’identificateur de cible de l’élément de calendrier ou de demande de réunion. 
    
2. Analyser les résultats de l’opération de **FindItem** (ou la méthode **Folder.FindItems** ) pour obtenir l’identificateur d’élément de l’élément de réunion. 
    
3. Utilisez l’opération EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir des objets de la réponse de la réunion. 
    
Le code XML suivant montre ce qui est envoyé pour demander des objets de la réponse sur un élément.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

La réponse d’opération **GetItem** ressemble au code XML suivant si vous avez demandé l’identificateur d’élément, le début de la réunion et l’heure de fin, la collection d’objets Response Group, et si l’organisateur autorise des modifications proposées à l’heure de la réunion. La collection d’objets de réponse, qui est représentée par l’élément [ResponseObjects](http://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , contient l’ensemble des réponses valides pour l’élément de calendrier. L’élément **ProposeNewTime** est un objet de réponse qui indique que l’utilisateur peut proposer une nouvelle heure pour la réunion. Les éléments [AcceptItem](http://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](http://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)et [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) représentent les objets de la réponse que vous pouvez utiliser pour proposer une nouvelle heure de réunion à l’organisateur de la réunion. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="propose-a-new-meeting-time-by-using-ews"></a>Proposer une nouvelle heure de réunion à l’aide de EWS
<a name="bk_Propose"> </a>

Si vous avez reçu d’un objet de réponse **ProposeNewTime** lorsque vous avez utilisé l’opération **GetItem** pour obtenir un élément de calendrier ou d’une demande de réunion, vous pouvez répondre avec une nouvelle heure de réunion. Si vous n’avez pas reçu un objet de réponse **ProposeNewTime** , vous ne pourrez plus proposer une nouvelle heure de réunion dans le cadre du flux de travail calendrier. Vous pouvez, toutefois, répondre à l’organisateur de la demande une nouvelle heure de réunion. Si vous recevez un objet de réponse **ProposeNewTime** , vous pouvez répondre à la réunion en faisant référence à son identificateur et proposer une nouvelle heure de réunion à l’organisateur de. Il s’agit de l’objet de réponse **ProposeNewTime** étant différente dans le modèle objet de réponse dans la mesure où vous ne répondez pas à un objet de réponse **ProposeNewTime** . Vous utilisez une des autres objets de réponse, telles que **AcceptItem**, **TentativelyAcceptItem**ou **DeclineItem**, de proposer une nouvelle réunion de la conférence. Cet exemple utilise l’objet de réponse **AcceptItem** . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

La réponse à cette requête contient l’identificateur de l’élément de calendrier qui a été ajoutée pour le calendrier du participant et une copie de la demande de réunion a été placée dans le dossier des éléments supprimés du participant. Le message de réponse avec la nouvelle proposition de temps a été également enregistré dans le dossier éléments envoyés du participant (vous devez trouver la réunion pour obtenir le handle sur ce message de réponse).
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

L’organisateur reçoit un message [MeetingResponse](http://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) lorsque le participant répond avec une nouvelle heure de réunion. Le message **MeetingResponse** contient la nouvelle réunion proposée heure de début et heure de fin et l’identificateur de l’élément de calendrier dans le calendrier de l’organisateur. L’organisateur peut utiliser ces informations pour mettre à jour leur élément existant du calendrier de la réunion. Vous trouverez ci-dessous le flux de travail pour l’organisateur répondre à un message **MeetingResponse** qui propose une nouvelle heure de réunion : 
  
1. Déterminer si les éléments **ProposedStart** ou **ProposedEnd** ont été définies dans le **MeetingResponse**. Dans ce cas, passez à l’étape 2. Si ce n’est pas le cas, le message **MeetingResponse** n'indique que le participant a accepté, provisoirement accepté ou refusé la réunion. 
    
2. Obtenir l’élément existant du calendrier de l’organisateur de la réunion à l’aide de l’identificateur EWS renvoyé dans l’élément **AssociatedCalendarItemId** . 
    
3. Comparez la démarrer d’origine et l’heure de fin avec la nouvelle heure de réunion. Si la nouvelle heure de réunion est acceptable pour l’organisateur, passez à l’étape 4. Sinon, l’organisateur de la réunion peut ignorer l’heure de réunion proposée, soit envoyer une réponse par courrier électronique sur le participant que vous avez choisi la nouvelle heure de réunion.
    
4. (Facultatif) Effectuer un appel de l’opération [GetUserAvailability](http://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS permettant de savoir si l’heure proposée fonctionnera pour tous les participants, y compris les boîtes aux lettres de salle et des ressources. (Vous pouvez également utiliser la méthode d’API managées [ExchangeService.GetUserAvailability](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) pour effectuer cette opération). 
    
5. L’organisateur peut mettre à jour leur réunion avec les heures de réunion proposée nouveau, puis envoyer les mises à jour à tous les participants à l’aide de l’opération EWS [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) (ou la méthode d’API managées [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) ). 
    
La figure suivante illustre le processus qui se produit entre l’organisateur de la réunion, le participant et le serveur Exchange qui gérés les appels EWS.
  
**La figure 1. Processus de proposition une nouvelle heure de réunion**

![La figure illustre le flux de travail entre l’organisateur, Exchange et un participant lorsqu’un nouvel horaire de réunion est proposé. Si l’organisateur autorise de nouvelles propositions de réunion, un participant peut proposer un nouvel horaire de réunion avec un objet de réponse.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a>Différences entre les versions
<a name="bk_Behavior"> </a>

La fonctionnalité de temps de nouveau proposer a été introduite dans Exchange correspond à la version 15.00.0800.007. Dans les versions antérieures d’Exchange, les utilisateurs d’applications EWS ont envoyer un message à l’organisateur de la réunion à demander une nouvelle date de réunion. 
  
## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

