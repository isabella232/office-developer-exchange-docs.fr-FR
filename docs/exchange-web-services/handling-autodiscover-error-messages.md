---
title: Gestion des messages d’erreur de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Découvrez les différents types d’erreurs de découverte automatique et que faire avec eux.
ms.openlocfilehash: fcafc799f4d35e92159d2913845474ecf7bc5657
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754782"
---
# <a name="handling-autodiscover-error-messages"></a>Gestion des messages d’erreur de découverte automatique

Découvrez les différents types d’erreurs de découverte automatique et que faire avec eux.
  
Découverte automatique permet à vos applications récupérer les informations de configuration automatiquement, et il fonctionne très. Toutefois, tout ne se passe toujours en fonction du plan. Examinons les erreurs courants qui peuvent se produire et comment vous pouvez gérer les afin de réduire la nécessité d’inviter l’utilisateur à configurer manuellement votre client.
  
## <a name="http-status-errors"></a>Erreurs d’état HTTP
<a name="bk_HttpErrors"> </a>

Le premier type d’erreur que vous pouvez rencontrer lors de l’envoi de demandes de découverte automatique est l’état HTTP. Si l’état HTTP dans votre réponse n’est pas 200 (OK), la charge utile de réponse ne contient pas la réponse de découverte automatique que vous recherchez. Par souci de simplicité, nous pouvons grouper les codes d’état non 200 en trois catégories.
  
**Le tableau 1. Codes d’état HTTP**

|**Code d’état**|**Type d’erreur**|**Pour gérer...**|
|:-----|:-----|:-----|
|301 ou 302  <br/> |Erreur de redirection  <br/> |Renvoyer votre demande à l’URI contenue dans l’en-tête de réponse HTTP ligne « emplacement ». Pour plus d’informations, voir [Gestion des erreurs de redirection](#bk_HandlingRedirects).  <br/> |
|401  <br/> |Erreur non autorisée  <br/> |Le [processus de découverte automatique](autodiscover-for-exchange.md) implique la tentative de plusieurs URL potentiels, vous pouvez obtenir cette sur une seule URL que suivant accepte vos informations d’identification. Pour cette raison, vous ne devez pas tenir compte une seule erreur 401 pour indiquer que les informations d’identification ne sont pas valides. Toutefois, si vous recevez des 401 erreurs à partir de plusieurs URL, vous souhaiterez invite l’utilisateur à entrer de nouveau leur mot de passe (si possible).  <br/> |
|N’importe quel autre état non-200  <br/> |Erreur de point de terminaison de découverte automatique non valide  <br/> |Prendre en compte l’URL qui renvoie un autre code d’état non 200 comme non valide et continue d’essayer de l’URL suivante dans votre liste.  <br/> |
   
## <a name="autodiscover-errors"></a>Erreurs de découverte automatique
<a name="bk_AutodiscoverErrors"> </a>

Même si vous obtenez un code d’état 200 (OK) après l’envoi d’une demande de découverte automatique, cela ne signifie pas que le serveur a envoyé les informations que nécessaires. L’état de 200 signifie simplement que vous avez une réponse de découverte automatique et réponse peut contenir une erreur dans la charge utile. L’emplacement des informations d’erreur diffère selon que le format est SOAP ou variole.
  
### <a name="soap-autodiscover-errors"></a>Erreurs de découverte automatique SOAP

Pour la découverte automatique SOAP, la réponse peut contenir un ou plusieurs éléments [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) dans plusieurs emplacements. En règle générale, vous pouvez tirer un élément enfant de l’élément de [Réponse (SOAP)](http://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) et un en tant qu’enfant de chaque élément de [Réponse utilisateur (SOAP)](http://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) dans la réponse. Vous pouvez également rencontrer un en tant qu’enfant d’un élément [UserSettingError (SOAP)](http://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , s’il est présent. Le contexte de l’erreur dépend de l’élément **ErrorCode** situe, comme suit : 
  
- Élément enfant de l’élément de **réponse** , l’élément **ErrorCode** représente une erreur qui s’applique à l’ensemble de la demande. 
    
- En tant qu’enfant de l’élément de **réponse utilisateur** , elle représente une erreur qui s’applique uniquement à un utilisateur spécifique. 
    
- En tant qu’enfant d’un élément **UserSettingError** , il représente une erreur qui s’applique à un paramètre spécifique qui a été demandé. 
    
Examinons un exemple d’une réponse. Dans cet exemple, l’élément **ErrorCode** sous l’élément de **réponse** a une valeur de « NoError », ce qui indique la réussite. Toutefois, l’élément **ErrorCode** sous l’élément de **réponse utilisateur** a une valeur de « RedirectAddress », ce qui indique qu’une erreur s’est produite pour cet utilisateur spécifique. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>elvin@mail.contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

L’article [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contient une liste complète des erreurs possibles. La plupart de ces indique une erreur irrécupérable, mais quelques justifient une gestion spéciale. 
  
**Le tableau 2. Valeurs Autodisover ErrorCode SOAP**

|**Valeur de code d’erreur**|**Pour gérer...**|
|:-----|:-----|
|RedirectAddress  <br/> |[Le redémarrage de la découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l’élément [RedirectTarget (SOAP)](http://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .  <br/> |
|RedirectUrl  <br/> |[Renvoi de votre demande vers une nouvelle URL](#bk_ResendRequest) à l’URL dans l’élément **RedirectTarget** .  <br/> |
|ServerBusy  <br/> |Réessayez cette URL après un court délai. Vous pouvez attendre un laps de temps ou simplement déplacer cette URL à la fin de la liste d’URL pour essayer. Si vous recevez cette erreur plusieurs fois à partir d’une URL, vous devez envisager l’URL non valide.  <br/> |
   
### <a name="pox-autodiscover-errors"></a>Erreurs de découverte automatique POX

Le service de découverte automatique variole signale les erreurs un peu différemment. Erreurs non récupérables sont contenues dans l’élément [Erreur (POX)](http://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) . L’article [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contient une liste complète des codes d’erreur possibles. 
  
Erreurs de redirection sont contenues dans l’élément [Action (POX)](http://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) . N’importe quelle valeur de l’élément **Action** autres que « paramètres » indique une erreur de redirection. 
  
**Le tableau 3. Valeurs Autodisover ErrorCode POX**

|**Valeur d’action**|**Pour gérer...**|
|:-----|:-----|
|redirectAddr  <br/> |[Le redémarrage de la découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l’élément [RedirectAddr (POX)](http://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .  <br/> |
|redirectUrl  <br/> |[Renvoi de votre demande vers une nouvelle URL](#bk_ResendRequest) à l’URL dans l’élément [RedirectUrl (POX)](http://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .  <br/> |
   
Dans cet exemple, l’élément **Action** a la valeur « redirectAddr », ce qui indique qu’une nouvelle demande doit être envoyée avec la nouvelle adresse de messagerie contenue dans l’élément **RedirectAddr** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>Gestion des erreurs de redirection
<a name="bk_HandlingRedirects"> </a>

Vous pouvez gérer des scénarios de redirection d’erreur de deux manières :
  
- En redémarrant la découverte automatique avec une nouvelle adresse de messagerie.
    
- Par le renvoi de votre demande vers une nouvelle URL.
    
Les deux scénarios nécessitent une validation avant de continuer.
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>Redémarrage du service de découverte automatique avec une nouvelle adresse de messagerie
<a name="bk_RestartAutodiscover"> </a>

Lorsque vous participez à une nouvelle adresse de messagerie une découverte automatique rediriger réponse, tout d’abord vérifier que la nouvelle adresse de messagerie qui a été fournie dans la réponse d’erreur de redirection n’est pas la même adresse que vous avez envoyé dans la demande qui a provoqué l’erreur. Si tel est le cas, vous ne devez pas redémarrer le service de découverte automatique et prendre en compte à la place de l’URL qui a généré la réponse comme non valide.
  
Si la nouvelle adresse de messagerie est différente, annuler votre liste existante d’URL de point de terminaison de découverte automatique potentiels et générer une nouvelle liste en fonction de la nouvelle adresse de messagerie.
  
### <a name="resending-your-request-to-a-new-url"></a>Renvoi de votre demande vers une nouvelle URL
<a name="bk_ResendRequest"> </a>

Lorsque vous recevez une nouvelle URL dans une réponse de redirection de découverte automatique, vous devez tout d’abord valider l’URL comme suit :
  
- Vérifiez que l’URL est une URL HTTPS.
    
- Vérifiez que vous n’avez pas reçu une erreur à partir de cette URL avec l’adresse de messagerie actuelle avant.
    
- Le cas échéant à votre application, informer l’utilisateur de la redirection et obtenez leur autorisation pour suivre la redirection.
    
- Envoyer une requête à l’URL et [Vérifiez que le certificat SSL présenté par le serveur est valid](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).
    
Si l’URL est validé, renvoyez la demande à cette nouvelle URL.
  
## <a name="see-also"></a>Voir aussi


- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)
    
- [Rechercher des points de terminaison de découverte automatique à l’aide de recherche SCP dans Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [ErrorCode (SOAP)](http://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [ErrorCode (POX)](http://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

