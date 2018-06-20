---
title: Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Découvrez la gestion de l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres.
ms.openlocfilehash: 7cfbfb5cc19e092c37e3d48a7fcc4f27023516e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754856"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Conserve les affinités entre un groupe d’abonnements et le serveur de boîtes aux lettres dans Exchange

Découvrez la gestion de l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres.
  
L’affinité est l’association d’une séquence de messages de demande et réponse avec un serveur de boîtes aux lettres spécifique. La plupart des fonctionnalités de Microsoft Exchange, l’affinité est gérée par le serveur. Notifications, toutefois, sont une exception. Le client est responsable de l’affinité avec le serveur de boîtes aux lettres pour les abonnements aux notifications. Cette affinité permet l’équilibreur de charge et les serveurs d’accès Client entre le client et le serveur pour les abonnements aux notifications itinéraire et requêtes connexes sur le serveur de boîtes aux lettres qui gère l’abonnement. Sans affinité, la demande routée vers un autre serveur de boîtes aux lettres qui n’inclut pas les abonnements aux informations du client, ce qui peuvent provoquer une erreur [ErrorSubscriptionNotFound](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) à renvoyer. 
  
## <a name="how-is-affinity-maintained"></a>Comment l’affinité est conservée ?
<a name="bk_howmaintained"> </a>

Affinité dans Exchange est basé le cookie. Le client déclenche la création du cookie en incluant des en-têtes spécifiques dans la demande d’abonnement, puis la réponse de l’abonnement contient le cookie. Le client envoie ensuite ce cookie dans les demandes suivantes pour vous assurer que la demande est routée vers le serveur de boîtes aux lettres de droite.
  
Plus précisément, l’affinité dans Exchange est gérée par les éléments suivants : 
  
- X-AnchorMailbox, En-tête HTTP une qui est inclus dans la demande initiale d’abonnement. Il identifie la première boîte aux lettres dans un groupe de boîtes aux lettres qui partagent une affinité avec le même serveur de boîtes aux lettres.
    
- X-PreferServerAffinity — Un en-tête HTTP qui est inclus dans la demande d’abonnement initial avec l’en-tête X-AnchorMailbox et est définie sur true pour indiquer que le client demande que l’affinité être mis à jour avec le serveur de boîtes aux lettres.
    
- X-BackEndOverrideCookie — Un cookie qui est inclus dans la réponse de l’abonnement initial et contient un cookie de l’équilibreur de charge et le serveur d’accès au Client permettent de router les demandes ultérieures sur le même serveur de boîtes aux lettres.
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a>Comment mettre à jour l’affinité à l’aide de l’API managée EWS ou EWS ?
<a name="bk_howdoimaintain"> </a>

Vous pouvez utiliser les mêmes étapes pour mettre à jour une affinité pour plusieurs abonnements de boîte aux lettres et de leurs serveurs de boîtes aux lettres, quel que soit le si vous utilisez une diffusion en continu, extraits ou les notifications push, et quelle que soit la si vous ciblez une Exchange serveur local ou Exchange Online.
  
1. Pour chaque boîte aux lettres, [appelez le service de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) et les paramètres utilisateur GroupingInformation et ExternalEwsUrl. Vous utilisez l’élément de [paramètre](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) pour la découverte automatique SOAP, et pour la découverte automatique variole, vous utilisez l’élément [GroupingInformation](http://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) . 
    
2. En utilisant les paramètres GroupingInformation et ExternalEwsUrl parmi les réponses de découverte automatique, place les boîtes aux lettres avec les mêmes GroupingInformation et ExternalEwsUrl concaténée valeur dans le même groupe. Si tous les groupes ont plus de 200 boîtes aux lettres, décomposer les groupes supplémentaires afin que chaque groupe ait pas plus de 200 boîtes aux lettres.
    
3. Créer et utiliser un seul objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) pour le reste de la procédure. Lorsque vous utilisez le même **ExchangeService** objet, les cookies et les en-têtes (lorsqu’ils sont définis) sont automatiquement mises à jour. Notez que si vous ne souhaitez pas les abonnements de diffusion en continu de groupe en une seule connexion, vous pouvez créer un objet **ExchangeService** différent pour chaque utilisateur représenté. 
    
4. [Envoyer un abonnement à](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) la demande de l’utilisateur dont le nom d’utilisateur s’affiche lorsque tous les utilisateurs dans le groupe sont triés par ordre alphabétique (nous allons faire référence à cet utilisateur que l’utilisateur de boîte aux lettres d’ancrage). Procédez comme suit : 
    
  - Inclure l’en-tête X-AnchorMailbox avec une valeur définie à l’adresse SMTP de l’utilisateur de boîte aux lettres d’ancrage.
    
  - Inclure l’en-tête X-PreferServerAffinity avec une valeur est définie sur true.
    
  - Utilisez le rôle [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (type [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
5. Dans la réponse de l’abonnement, obtenez la valeur X-BackEndOverrideCookie. Inclure cette valeur dans chacun des demandes d’abonnement suivantes pour les utilisateurs de ce groupe.
    
6. Pour chaque utilisateur dans le groupe, envoyez une demande d’abonnement et procédez comme suit :
    
  - Inclure l’en-tête X-AnchorMailbox avec une valeur définie à l’adresse SMTP de l’utilisateur de boîte aux lettres d’ancrage pour le groupe.
    
  - Inclure l’en-tête X-PreferServerAffinity avec une valeur est définie sur true.
    
  - Inclure le X-BackEndOverrideCookie qui a été retournée dans la réponse d’abonnement de l’utilisateur de boîte aux lettres d’ancrage.
    
  - Utilisez le rôle [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (type [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
    Notez que le serveur utilise les valeurs X-PreferServerAffinity et X-BackendOverrideCookie ensemble pour effectuer le routage vers le serveur de boîtes aux lettres. L’en-tête X-AnchorMailbox est également requis, mais est ignorée par le serveur si les deux valeurs sont valides. Si X-AnchorMailbox et X-PreferServerAffinity se trouvent dans une demande et X-BackendOverrideCookie n’est pas inclus, la valeur X-AnchorMailbox est utilisée pour router les demandes.
    
    Étant donné que les valeurs X-BackendOverrideCookie X-PreferServerAffinity effectuent le routage, si la boîte aux lettres d’ancrage jamais déplace vers un autre groupe ou serveur, la logique ne change pas, car le X-BackendOverrideCookie achemine la demande vers le serveur approprié pour le groupe.
    
7. Envoyer un seul [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou demandes [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) pour le groupe et procédez comme suit : 
    
  - Inclure les valeurs de [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) retournées dans chacun des réponses abonnement individuels pour les boîtes aux lettres dans le groupe. 
    
  - Si plus de 200 abonnements existent pour le groupe, créer plusieurs demandes. Le nombre maximal de valeurs [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) à inclure dans une requête est 200. 
    
  - Si vous avez besoin de plus de connexions sont disponibles pour la boîte aux lettres cible, utilisez le compte de service pour emprunter l’identité de la boîte aux lettres d’ancrage pour le groupe ; Sinon, n’utilisez pas l’emprunt d’identité. Dans l’idéal, vous souhaitez emprunter l’identité d’une boîte aux lettres unique par demande [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) ou [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) afin que vous rencontrez jamais les limites de limitation. 
    
  - Utilisez ApplicationImpersonation si vous avez besoin de [plus de connexions sont disponibles pour la boîte aux lettres cible](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); Sinon, n’utilisez pas ApplicationImpersonation.
    
  - Inclure l’en-tête X-PreferServerAffinity et affectez-lui la valeur true. Cette valeur est automatiquement incluse si vous utilisez l’objet **ExchangeService** que vous avez créé à l’étape 2. 
    
  - Inclure le X-BackEndOverrideCookie pour le groupe (le X-BackEndOverrideCookie qui a été retournée dans la réponse d’abonnement de l’utilisateur de boîte aux lettres d’ancrage). Cette valeur est automatiquement incluse si vous utilisez l’objet **ExchangeService** que vous avez créé à l’étape 2. 
    
8. Transmettre les événements renvoyés vers un thread distinct pour traitement.
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>Les valeurs de limitation ai-je besoin de prendre en considération ?
<a name="bk_throttling"> </a>

Lorsque vous planifiez votre implémentation de notification, vous souhaiterez tenir compte des deux valeurs : le nombre de connexions et le nombre d’abonnements. Le tableau suivant répertorie les valeurs par défaut pour chaque paramètre [de limitation](ews-throttling-in-exchange.md) et la façon dont les paramètres sont utilisés. Pour chaque valeur, le budget est affecté à la boîte aux lettres cible. Pour cette raison, à l’aide de l’emprunt d’identité pour obtenir des connexions supplémentaires est une étape obligatoire dans de nombreux scénarios. 
  
**Le tableau 1. Limitation des valeurs par défaut**

|**Zone de compte**|**Paramètres de limitation**|**Valeur par défaut**|**Description**|
|:-----|:-----|:-----|:-----|
|Connexions de diffusion en continu  <br/> |Par défaut négatif la limite de connexion  <br/> |10 pour Exchange Online  <br/> 3 pour Exchange 2013  <br/> |Le nombre maximal de connexions simultanées en continu ayant un compte peut ouvre en même temps sur le serveur. Pour travailler au sein de cette limite, utilisez un compte de service avec le rôle ApplicationImpersonation pour les boîtes aux lettres cible et emprunter l’identité du premier utilisateur dans chaque groupe de ID d’abonnement lors de l’obtention de diffusée en continu des événements.  <br/> |
|Connexions pull ou push  <br/> |EWSMaxConcurrency  <br/> |27  <br/> |Le nombre maximal de connexions simultanées de type pull ou push (demandes qui ont été reçus mais pas encore répondus) qui un compte permettre être ouverts sur le serveur en même temps.  <br/> |
|Abonnements  <br/> |EWSMaxSubscriptions  <br/> |20 pour Exchange Online  <br/> 5000 pour Exchange 2013  <br/> |Le nombre maximal d’abonnements nonexpired ayant un compte peut en même temps. Cette valeur est diminue lorsque l’abonnement est créé sur le serveur.  <br/> |
   
L’exemple suivant montre comment les budgets sont gérés entre une boîte aux lettres cible et le compte de service qui a le rôle [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) pour les boîtes aux lettres cible. 
  
- ServiceAccount1 (sa1) emprunte l’identité du nombre d’utilisateurs (m1, m2, m3 et ainsi de suite) et crée des abonnements pour chaque boîte aux lettres. Notez que lorsque les abonnements sont créés, le propriétaire de l’abonnement est sa1, afin que lorsque sa1 ouvre une connexion avec les abonnements, EWS impose que les abonnements sont détenues par sa1.
    
- Sa1 peut ouvrir la connexion de la manière suivante :
    
1. Sans l’emprunt d’identité, donc la connexion est chargée par rapport à sa1.
    
2. À l’emprunt d’identité des utilisateurs — m1, par exemple, afin que la connexion est facturée par rapport à une copie du budget de m1. (M1 lui-même peut ouvrir des dix connexions via Exchange Online et tous les comptes de service à emprunt d’identité m1 peuvent ouvrir des dix connexions à l’aide du budget copié.)
    
- Si la limite de connexion est atteint, les solutions de contournement suivantes sont disponibles :
    
  - Si l’option 1 est utilisée, l’administrateur peut créer plusieurs comptes de service pour emprunter l’identité des utilisateurs.
    
  - Si l’option 2 est utilisée, le code peut emprunter l’identité d’un autre utilisateur, m2 par exemple.
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>Exemple : Gestion de l’affinité entre un groupe d’abonnements et le serveur de boîtes aux lettres
<a name="bk_ce"> </a>

OK, nous allons le voir en action. L’exemple de code suivant montre comment les utilisateurs de groupe et permet de gérer l’affinité avec le serveur de boîtes aux lettres les en-têtes X-AnchorMailbox et X-PreferServerAffinity et le cookie X-BackendOverrideCookie. Les en-têtes et étant le cookie d’avancement de l’histoire de l’affinité, cet exemple montre comment se concentre sur les demandes EWS XML et les réponses. Pour créer le corps des demandes d’abonnement et des réponses à l’aide de l’API managée EWS, voir [notifications de flux de données sur les événements de boîte aux lettres à l’aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) et [extraire les notifications concernant les événements de boîte aux lettres à l’aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). Cette section inclut notamment des étapes supplémentaires pour maintenir l’affinité et en ajoutant les en-têtes à vos demandes.
  
Cet exemple comporte quatre utilisateurs : alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com et sadie@contoso.com. La figure suivante illustre le GroupingInformation et ExternalEwsUrl [paramètres de découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) pour les utilisateurs. 
  
**La figure 1. Paramètres de découverte automatique permet de boîtes aux lettres de groupe**

![Table illustrant les valeurs GroupingInformation et ExternalEwsUrl pour chacun des utilisateurs.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
Utiliser les paramètres de réponses de la découverte automatique, les boîtes aux lettres sont regroupés par la valeur concaténée des paramètres GroupingInformation et ExternalEwsUrl. Dans cet exemple, Alfred et Sadie ont les mêmes valeurs, afin qu’ils sont dans un groupe, et Alisa et Ronnie partagent les mêmes valeurs, ils se trouvent dans un autre groupe.
  
**La figure 2. Création de groupes de boîtes aux lettres**

![Tableau illustrant la création des groupes de boîtes aux lettres à l’aide des paramètres de découverte automatique.](media/Exchange2013_NotificationAffinityGrouping.png)
  
Pour les besoins de cet exemple, nous nous concentrerons sur le groupe A. Nous utiliser les mêmes étapes pour le groupe B, mais les utiliser une autre valeur X-AnchorMailbox pour ce groupe.
  
À l’aide [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx), créer la demande d’abonnement pour la boîte aux lettres d’ancrage (alfred@contoso.com), avec l’en-tête X-AnchorMailbox défini le leur adresse de messagerie et une valeur de l’en-tête X-PreferServerAffinity de la valeur true. Définition des valeurs de ces deux en-tête déclenche le serveur pour créer un X-BackEndOverrideCookie pour la réponse.
  
Si vous utilisez l’API managée EWS, utilisez la méthode[Add](http://msdn.microsoft.com/EN-US/library/cy7xta5e) [en-têtes](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)pour ajouter les en-têtes de deux à votre demande d’abonnement, comme indiqué. 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

Donc demande d’abonnement de Alfred se présente comme suit.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le message XML suivant est la réponse à la demande d’abonnement de Alfred, et il inclut la X-BackEndOverrideCookie. Renvoyer ce cookie pour toutes les requêtes suivantes pour les utilisateurs de ce groupe. Notez que la réponse contienne également des cookies supplémentaires, telles que le cookie exchangecookie utilisés par Exchange 2010. Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions d’Exchange commençant par Exchange 2013, ignorer exchangecookie si elle est incluse dans les demandes d’abonnement suivantes.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

À l’aide de la X-BackEndOverrideCookie à partir de la réponse de Alfred et l’en-tête X-AnchorMailbox, la demande d’abonnement est créée pour Sadie, l’autre membre de la demande d’abonnement de Sadie groupe A. se présente comme suit.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@consoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@consoso.com </t:SmtpAddress>
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

Réponse d’abonnement de Sadie se présente comme suit. Notez qu’il ne comprend pas le X-BackEndOverrideCookie. Le client est chargé de la mise en cache de cette valeur pour les demandes ultérieures.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Une demande d’opération [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) les valeurs à partir des réponses de l’abonnement a été créée pour tous les abonnements dans le groupe. Car il y a moins de 200 abonnements dans ce groupe, elles sont toutes envoyées dans une requête. L’en-tête X-PreferServerAffinity est défini sur true et la X-BackEndOverrideCookie est inclus. 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Les événements retournés sont ensuite transmis à un thread distinct pour le traitement.
  
## <a name="how-has-affinity-changed"></a>Comment l’affinité a changé ?
<a name="bk_howchanged"> </a>

Dans Exchange 2010, les abonnements sont conservés sur le serveur d’accès au Client, comme le montre la Figure 3. Dans les versions d’Exchange Exchange 2010 au plus tard, les abonnements sont conservés sur le serveur de boîtes aux lettres, comme le montre la Figure 4.
  
**La figure 3. Processus de maintien de l’affinité dans Exchange 2010**

![Illustration présentant la façon dont la table d’abonnements actifs est conservée sur le serveur d’accès au client dans Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
**La figure 4. Processus de maintien de l’affinité dans Exchange Online et Exchange 2013**

![Illustration présentant la façon dont l’équilibrage de charge et le serveur d’accès au client acheminent les demandes vers le serveur de boîtes aux lettres qui conserve la table des abonnements actifs dans Exchange Server et Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
Dans Exchange 2010, le client seulement sait l’adresse de l’équilibrage de charge et l’exchangecookie renvoyée par le serveur garantit que la demande est routée vers le serveur d’accès au Client droite. Toutefois, dans les versions ultérieures, l’équilibrage de charge et les rôles de serveur d’accès au Client ont router les demandes de manière appropriée avant qu’ils n’atteignent le serveur de boîtes aux lettres. Pour faire que des informations supplémentaires sont nécessaires, c’est pourquoi les nouveaux en-têtes et les cookies ont été apportées. La [Notification d’abonnements, les événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) explique comment les abonnements sont conservées dans Exchange 2013. 
  
Vous pouvez remarquer que l’exchangecookie qui utilise Exchange 2010 est toujours retourné par une version ultérieure. Il n’existe aucun dommage, y compris ce cookie dans les requêtes, mais ignorent les versions ultérieures d’Exchange.
  
## <a name="see-also"></a>Voir aussi

- [Abonnements à des notifications, événements de boîte aux lettres et EWS dans Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Notifications de flux de données sur les événements de boîte aux lettres à l’aide de EWS dans Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Extraction des notifications concernant les événements de boîte aux lettres à l’aide de EWS dans Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Gestion des erreurs liées à la notification dans EWS dans Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
- [Modifications dans la gestion de l’affinité pour les abonnements EWS...](http://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [Limitation EWS dans Exchange](ews-throttling-in-exchange.md)
    

