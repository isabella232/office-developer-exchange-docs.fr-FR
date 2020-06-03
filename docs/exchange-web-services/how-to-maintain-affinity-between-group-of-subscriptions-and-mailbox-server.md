---
title: Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Découvrez comment maintenir l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres.
localization_priority: Priority
ms.openlocfilehash: 1618216cf69e08b2ae774264e0910856a59851af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44455756"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Conserver l’affinité entre un groupe d'abonnements et le serveur de boîtes aux lettres dans Exchange

Découvrez comment maintenir l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres.
  
L’affinité est l’Association d’une séquence de messages de demande et de réponse à un serveur de boîtes aux lettres particulier. Pour la plupart des fonctionnalités dans Exchange, l’affinité est gérée par le serveur. Toutefois, les notifications sont des exceptions. Le client est responsable de la maintenance de l’affinité avec le serveur de boîtes aux lettres pour les abonnements aux notifications. Cette affinité active l’équilibreur de charge et les serveurs d’accès au client entre le client et le serveur pour acheminer les abonnements aux notifications et les demandes associées vers le serveur de boîtes aux lettres qui gère l’abonnement. Sans affinité, la demande peut être acheminée vers un autre serveur de boîtes aux lettres qui n’inclut pas les abonnements du client, ce qui peut entraîner le renvoi d’une erreur [ErrorSubscriptionNotFound](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) . 
  
## <a name="how-is-affinity-maintained"></a>Comment l’affinité est-elle conservée ?
<a name="bk_howmaintained"> </a>

L’affinité dans Exchange est basée sur les cookies. Le client déclenche la création du cookie en incluant des en-têtes spécifiques dans la demande d’abonnement, puis la réponse de l’abonnement contient le cookie. Le client envoie ensuite ce cookie dans les demandes suivantes pour s’assurer que la demande est routée vers le serveur de boîtes aux lettres approprié.
  
Plus spécifiquement, l’affinité dans Exchange est gérée par les éléments suivants : 
  
- X-AnchorMailbox : en-tête HTTP inclus dans la demande d’abonnement initiale. Il identifie la première boîte aux lettres d’un groupe de boîtes aux lettres qui partagent l’affinité avec le même serveur de boîtes aux lettres.
    
- X-PreferServerAffinity : en-tête HTTP inclus dans la demande d’abonnement initiale avec l’en-tête X-AnchorMailbox et est défini sur true pour indiquer que le client demande que l’affinité soit maintenue avec le serveur de boîtes aux lettres.
    
- X-BackEndOverrideCookie — cookie inclus dans la réponse d’abonnement initiale et contenant un cookie que l’équilibreur de charge et le serveur d’accès au client utilisent pour acheminer les demandes ultérieures vers le même serveur de boîtes aux lettres.
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a>Comment puis-je conserver les affinités à l’aide de l’API managée EWS ou EWS ?
<a name="bk_howdoimaintain"> </a>

Vous pouvez utiliser les mêmes étapes pour conserver l’affinité pour les abonnements à plusieurs boîtes aux lettres et leurs serveurs de boîtes aux lettres, que vous utilisiez des notifications de diffusion en continu, d’extraction ou de transmission, et que vous cibliez ou non un serveur Exchange local ou Exchange Online.
  
1. Pour chaque boîte aux lettres, [appelez Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et obtenez les paramètres utilisateur GroupingInformation et ExternalEwsUrl. Pour la découverte automatique SOAP, vous utilisez l’élément [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) et pour la découverte automatique POX, vous utilisez l’élément [GroupingInformation](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) . 
    
2. En utilisant les paramètres GroupingInformation et ExternalEwsUrl des réponses de découverte automatique, placez les boîtes aux lettres avec la même valeur concaténée ExternalEwsUrl et GroupingInformation dans le même groupe. Si des groupes possèdent plus de 200 boîtes aux lettres, Rompez-les davantage afin que chaque groupe ne contienne pas plus de 200 boîtes aux lettres.
    
3. Créez et utilisez un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) pour le reste de la procédure. Lorsque vous utilisez le même objet **ExchangeService** , les cookies et les en-têtes (lorsqu’ils sont définis) sont automatiquement gérés. Notez que si vous n’avez pas l’intention de regrouper des abonnements de diffusion en continu dans une seule connexion, vous pouvez créer un objet **ExchangeService** différent pour chaque utilisateur emprunté. 
    
4. [Envoyer une](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) demande d’abonnement pour l’utilisateur dont le nom d’utilisateur apparaît en premier lorsque tous les utilisateurs du groupe sont triés par ordre alphabétique (nous faisons référence à cet utilisateur comme l’utilisateur de la boîte aux lettres d’ancrage). Procédez comme suit : 
    
  - Incluez l’en-tête X-AnchorMailbox avec une valeur définie sur l’adresse SMTP de l’utilisateur de la boîte aux lettres d’ancrage.
    
  - Incluez l’en-tête X-PreferServerAffinity avec une valeur définie sur true.
    
  - Utilisez le rôle [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (type [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
5. Dans la réponse de l’abonnement, obtenez la valeur X-BackEndOverrideCookie. Incluez cette valeur dans chacune des demandes d’abonnements suivantes pour les utilisateurs de ce groupe.
    
6. Pour chaque utilisateur supplémentaire dans le groupe, envoyez une demande d’abonnement et procédez comme suit :
    
  - Incluez l’en-tête X-AnchorMailbox avec une valeur définie sur l’adresse SMTP de l’utilisateur de la boîte aux lettres d’ancrage du groupe.
    
  - Incluez l’en-tête X-PreferServerAffinity avec une valeur définie sur true.
    
  - Incluez la X-BackEndOverrideCookie qui a été renvoyée dans la réponse de l’utilisateur de la boîte aux lettres d’ancrage.
    
  - Utilisez le rôle [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (type [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
    Notez que le serveur utilise les valeurs X-PreferServerAffinity et X-BackendOverrideCookie pour effectuer le routage vers le serveur de boîtes aux lettres. L’en-tête X-AnchorMailbox est également requis, mais est ignoré par le serveur si les deux autres valeurs sont valides. Si X-AnchorMailbox et X-PreferServerAffinity sont dans une requête et que X-BackendOverrideCookie n’est pas inclus, la valeur X-AnchorMailbox est utilisée pour acheminer les demandes.
    
    Étant donné que les valeurs X-PreferServerAffinity et X-BackendOverrideCookie effectuent le routage, si la boîte aux lettres d’ancrage ne passe pas à un autre groupe ou serveur, la logique ne change pas, car X-BackendOverrideCookie achemine la demande vers le serveur approprié pour le groupe.
    
7. Envoyez une seule demande [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) pour le groupe, puis procédez comme suit : 
    
  - Incluez les valeurs [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) renvoyées dans chacune des réponses d’abonnement individuelles pour les boîtes aux lettres du groupe. 
    
  - Si plus de 200 abonnements existent pour le groupe, créez plusieurs demandes. Le nombre maximal de valeurs [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) à inclure dans une demande est de 200. 
    
  - Si vous avez besoin de plus de connexions que celles disponibles pour la boîte aux lettres cible, utilisez le compte de service pour emprunter l’identité de la boîte aux lettres d’ancrage du groupe ; Sinon, n’utilisez pas l’emprunt d’identité. Idéalement, vous souhaitez emprunter l’identité d’une boîte aux lettres unique par demande [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) afin de ne pas rencontrer de limites de limitation. 
    
  - Utilisez ApplicationImpersonation si vous avez besoin de [plus de connexions que celles disponibles pour la boîte aux lettres cible](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); Sinon, n’utilisez pas ApplicationImpersonation.
    
  - Incluez l’en-tête X-PreferServerAffinity et définissez-le sur true. Cette valeur est incluse automatiquement si vous utilisez l’objet **ExchangeService** que vous avez créé à l’étape 2. 
    
  - Incluez X-BackEndOverrideCookie pour le groupe (X-BackEndOverrideCookie qui a été renvoyé dans la réponse d’abonnement de l’utilisateur de la boîte aux lettres d’ancrage). Cette valeur est incluse automatiquement si vous utilisez l’objet **ExchangeService** que vous avez créé à l’étape 2. 
    
8. Transmettez les événements renvoyés à un thread distinct pour traitement.
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>Quelles valeurs de limitation dois-je prendre en considération ?
<a name="bk_throttling"> </a>

Lorsque vous planifiez l’implémentation de vos notifications, vous devez prendre deux valeurs en considération : le nombre de connexions et le nombre d’abonnements. Le tableau suivant répertorie les valeurs par défaut pour chaque paramètre de [limitation](ews-throttling-in-exchange.md) et la façon dont les paramètres sont utilisés. Pour chaque valeur, le budget est alloué à la boîte aux lettres cible. Pour cette raison, l’utilisation de l’emprunt d’identité pour obtenir des connexions supplémentaires est une étape requise dans de nombreux scénarios. 
  
**Tableau 1. Valeurs de limitation par défaut**

|**Domaine de réflexion**|**Paramètre de limitation**|**Valeur par défaut**|**Description**|
|:-----|:-----|:-----|:-----|
|Connexions de diffusion en continu  <br/> |Limite de blocage par défaut  <br/> |10 pour Exchange Online  <br/> 3 pour Exchange 2013  <br/> |Nombre maximal de connexions de diffusion en continu simultanées qu’un compte peut ouvrir simultanément sur le serveur. Pour travailler dans cette limite, utilisez un compte de service avec le rôle ApplicationImpersonation attribué pour les boîtes aux lettres cibles et empruntez l’identité du premier utilisateur dans chaque groupe d’ID d’abonnement lors de l’obtention d’événements en flux.  <br/> |
|Connexions d’extraction ou de transmission par émission  <br/> |EWSMaxConcurrency  <br/> |vingt  <br/> |Nombre maximal de connexions d’extraction ou de transmission simultanées (demandes reçues mais pas encore satisfaites) qu’un compte peut ouvrir simultanément sur le serveur.  <br/> |
|Abonnements  <br/> |EWSMaxSubscriptions  <br/> |20 pour Exchange Online  <br/> 5000 pour Exchange 2013  <br/> |Nombre maximal d’abonnements non expirés qu’un compte peut avoir à la fois. Cette valeur est décrémentée lors de la création de l’abonnement sur le serveur.  <br/> |
   
L’exemple suivant montre comment les budgets sont gérés entre n’importe quelle boîte aux lettres cible et le compte de service auquel le rôle [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) est attribué pour les boîtes aux lettres cibles. 
  
- ServiceAccount1 (SA1) emprunte un grand nombre d’utilisateurs (M1, m2, m3, etc.) et crée des abonnements pour chaque boîte aux lettres. Notez que lorsque les abonnements sont créés, le propriétaire de l’abonnement est SA1, donc lorsque SA1 ouvre une connexion avec les abonnements, EWS applique que les abonnements appartiennent à SA1.
    
- SA1 peut ouvrir la connexion de l’une des manières suivantes :
    
1. Sans emprunt d’identité, la connexion est donc facturée par rapport à SA1.
    
2. En empruntant l’identité de l’un des utilisateurs (M1, par exemple) de sorte que la connexion soit facturée par rapport à une copie du budget m1's. (M1 elle-même peut ouvrir dix connexions à l’aide d’Exchange Online, et tous les comptes de service qui empruntent l’identité M1 peuvent ouvrir dix connexions à l’aide du budget copié.)
    
- Si la limite de connexion est atteinte, les solutions de contournement suivantes sont disponibles :
    
  - Si l’option 1 est utilisée, l’administrateur peut créer plusieurs comptes de service pour emprunter l’identité d’utilisateurs supplémentaires.
    
  - Si l’option 2 est utilisée, le code peut emprunter l’identité d’un autre utilisateur (m2 par exemple).
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>Exemple : conservation de l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres
<a name="bk_ce"> </a>

OK, voyons-le en action. L’exemple de code suivant montre comment regrouper des utilisateurs et utiliser les en-têtes X-AnchorMailbox et X-PreferServerAffinity et le cookie X-BackendOverrideCookie pour maintenir l’affinité avec le serveur de boîtes aux lettres. Étant donné que les en-têtes et le cookie ont une importance essentielle dans la histoire de l’affinité, cet exemple se concentre sur les requêtes et les réponses XML EWS. Pour utiliser l’API managée EWS afin de créer le corps des demandes et des réponses d’abonnement, consultez la rubrique [transmettre des notifications sur les événements de boîte aux lettres à l’aide d’EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) et les [notifications pull sur les événements de boîte aux lettres à l’aide d’EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). Cette section comprend des étapes supplémentaires en particulier pour conserver l’affinité et ajouter les en-têtes à vos demandes.
  
Cet exemple est doté de quatre utilisateurs : alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com et sadie@contoso.com. La figure suivante illustre les [paramètres de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) GroupingInformation et ExternalEwsUrl pour les utilisateurs. 
  
**Figure 1. Paramètres de découverte automatique utilisés pour regrouper des boîtes aux lettres**

![Table illustrant les valeurs GroupingInformation et ExternalEwsUrl pour chacun des utilisateurs.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
À l’aide des paramètres des réponses de découverte automatique, les boîtes aux lettres sont regroupées par la valeur concaténée des paramètres GroupingInformation et ExternalEwsUrl. Dans cet exemple, Alfred et Sadie ont les mêmes valeurs, de sorte qu’elles se trouvent dans un groupe et que Alisa et Ronnie partagent les mêmes valeurs, ils sont donc dans un autre groupe.
  
**Figure 2. Création de groupes de boîtes aux lettres**

![Tableau illustrant la création des groupes de boîtes aux lettres à l’aide des paramètres de découverte automatique.](media/Exchange2013_NotificationAffinityGrouping.png)
  
Dans le cadre de cet exemple, nous allons nous concentrer sur le groupe A. Nous allons utiliser les mêmes étapes pour le groupe B, mais utiliser une valeur X-AnchorMailbox différente pour ce groupe.
  
À l’aide de [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx), créez la demande d’abonnement pour la boîte aux lettres d’ancrage (Alfred@contoso.com), avec l’en-tête x-AnchorMailbox défini sur l’adresse de messagerie et une valeur d’en-tête x-PreferServerAffinity de true. La définition de ces deux valeurs d’en-tête déclenche le serveur pour créer une X-BackEndOverrideCookie pour la réponse.
  
Si vous utilisez l’API managée EWS, utilisez la méthode[Add](https://msdn.microsoft.com/library/cy7xta5e) [HttpHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)pour ajouter les deux en-têtes à votre demande d’abonnement, comme illustré. 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

Ainsi, la demande d’abonnement à Alfred se présente comme suit.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

Le message XML suivant est la réponse à la demande d’abonnement à Alfred, qui inclut X-BackEndOverrideCookie. Renvoyez ce cookie pour toutes les demandes suivantes pour les utilisateurs de ce groupe. Notez que la réponse contient également des cookies supplémentaires, tels que le cookie exchangecookie utilisé par Exchange 2010. Exchange Online, Exchange Online dans le cadre d’Office 365 et versions d’Exchange à partir d’Exchange 2013, ignorez exchangecookie s’il est inclus dans les demandes d’abonnement ultérieures.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

À l’aide de X-BackEndOverrideCookie à partir de la réponse de Alfred et de l’en-tête X-AnchorMailbox, la demande d’abonnement est créée pour Sadie, l’autre membre de la demande d’abonnement de groupe A. Sadie ressemble à ceci.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

La réponse d’abonnement de Sadie ressemble à ceci. Notez qu’il n’inclut pas X-BackEndOverrideCookie. Le client est responsable de la mise en cache de cette valeur pour les demandes ultérieures.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

À l’aide des valeurs [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) des réponses d’abonnement, une demande d’opération [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) a été créée pour tous les abonnements dans le groupe. Étant donné qu’il y a moins de 200 abonnements dans ce groupe, ils sont tous envoyés dans une demande. L’en-tête X-PreferServerAffinity est défini sur true et l’X-BackEndOverrideCookie est inclus. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

Les événements renvoyés sont ensuite transmis à un thread distinct pour traitement.
  
## <a name="how-has-affinity-changed"></a>Quelles sont les modifications apportées à l’affinité ?
<a name="bk_howchanged"> </a>

Dans Exchange 2010, les abonnements sont conservés sur le serveur d’accès au client, comme illustré dans la figure 3. Dans les versions d’Exchange ultérieures à Exchange 2010, les abonnements sont conservés sur le serveur de boîtes aux lettres, comme le montre la figure 4.
  
**Figure 3. Processus de conservation de l’affinité dans Exchange 2010**

![Illustration présentant la façon dont la table d’abonnements actifs est conservée sur le serveur d’accès au client dans Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
**Figure 4. Processus de conservation de l’affinité dans Exchange Online et Exchange 2013**

![Illustration présentant la façon dont l’équilibrage de charge et le serveur d’accès au client acheminent les demandes vers le serveur de boîtes aux lettres qui conserve la table des abonnements actifs dans Exchange Server et Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
Dans Exchange 2010, le client connaît uniquement l’adresse de l’équilibreur de charge et le exchangecookie renvoyé par le serveur s’assure que la demande est routée vers le serveur d’accès au client approprié. Toutefois, dans les versions ultérieures, les rôles du serveur d’accès au client et de l’équilibreur de charge doivent tous deux acheminer les demandes de manière appropriée avant qu’ils n’obtiennent le serveur de boîtes aux lettres. Pour ce faire, des informations supplémentaires sont requises, c’est pourquoi les nouveaux en-têtes et les cookies ont été introduits. L’article [abonnements aux notifications, les événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explique comment les abonnements sont gérés dans Exchange 2013. 
  
Vous pouvez remarquer que le exchangecookie utilisé par Exchange 2010 est toujours renvoyé par les versions ultérieures. Il n’y a aucun dommage à inclure ce cookie dans les requêtes, mais les versions ultérieures d’Exchange l’ignorent.
  
## <a name="see-also"></a>Voir aussi

- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Notifications de flux concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Notifications de type pull concernant les événements de boîte aux lettres à l'aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
- [Modifications apportées à la gestion de l’affinité pour les abonnements EWS...](https://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

