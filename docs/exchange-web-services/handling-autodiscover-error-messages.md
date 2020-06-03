---
title: Gestion des messages d'erreur de découverte automatique
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: e5939ec2-1100-4174-8a88-5a6e09b60b23
description: Découvrez les différents types d’erreurs de découverte automatique et la marche à suivre.
localization_priority: Priority
ms.openlocfilehash: 0cba7e54cb251a9775e0971826560e277dcd9d2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455960"
---
# <a name="handling-autodiscover-error-messages"></a>Gestion des messages d'erreur de découverte automatique

Découvrez les différents types d’erreurs de découverte automatique et la marche à suivre.
  
La découverte automatique permet à vos applications de récupérer automatiquement les informations de configuration et elle fonctionne parfaitement. Toutefois, les choses ne sont pas toujours conformes à la planification. Examinons les erreurs courantes susceptibles de se produire et vous pouvez les gérer afin de réduire le besoin d’inviter votre utilisateur à configurer manuellement votre client.
  
## <a name="http-status-errors"></a>Erreurs d’état HTTP
<a name="bk_HttpErrors"> </a>

Le premier type d’erreur que vous pouvez rencontrer lors de l’envoi de demandes de découverte automatique est l’état HTTP. Si l’état HTTP de votre réponse est autre que 200 (OK), la charge utile de la réponse ne contient pas la réponse de découverte automatique que vous recherchez. Par souci de simplicité, nous pouvons regrouper les codes d’État non 200 en trois catégories.
  
**Tableau 1. Codes d’état HTTP**

|**Code d’état**|**Type d’erreur**|**Pour gérer...**|
|:-----|:-----|:-----|
|301 ou 302  <br/> |Erreur de redirection  <br/> |Renvoyez votre requête à l’URI contenu dans l’en-tête de réponse HTTP « location ». Pour plus d’informations, consultez [la rubrique gestion des erreurs de redirection](#bk_HandlingRedirects).  <br/> |
|401  <br/> |Erreur non autorisée  <br/> |Étant donné que le [processus de découverte automatique](autodiscover-for-exchange.md) implique de tenter plusieurs URL potentielles, vous pouvez obtenir cette URL sur une seule URL pour qu’elle accepte vos informations d’identification. Pour cette raison, vous ne devez pas prendre en compte une seule erreur 401 pour indiquer que les informations d’identification ne sont pas valides. Toutefois, si vous recevez des erreurs 401 à partir de plusieurs URL, vous pouvez inviter l’utilisateur à entrer de nouveau son mot de passe (le cas échéant).  <br/> |
|Tout autre État autre qu' 200  <br/> |Erreur de point de terminaison de découverte automatique non valide  <br/> |Considérez l’URL qui renvoie tout autre code d’État non 200 comme non valide et continuez à essayer l’URL suivante dans votre liste.  <br/> |
   
## <a name="autodiscover-errors"></a>Erreurs de découverte automatique
<a name="bk_AutodiscoverErrors"> </a>

Même si vous obtenez un code d’état 200 (OK) après avoir envoyé une demande de découverte automatique, cela ne signifie pas que le serveur a envoyé les informations dont vous avez besoin. L’état 200 uniquement signifie que vous avez une réponse de découverte automatique et que cette réponse peut contenir une erreur au sein de la charge utile. L’emplacement des informations relatives à l’erreur diffère selon que le format est SOAP ou POX.
  
### <a name="soap-autodiscover-errors"></a>Erreurs de découverte automatique SOAP

Pour la découverte automatique SOAP, la réponse peut contenir un ou plusieurs éléments [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) , à différents endroits. En règle générale, vous pouvez vous attendre à ce qu’il s’agit d’un élément enfant de l’élément de [réponse (SOAP)](https://msdn.microsoft.com/library/4c2bcdeb-95ce-4ffa-bd83-118af53b534f%28Office.15%29.aspx) et de l’autre en tant qu’enfant de chaque élément [UserResponse (SOAP)](https://msdn.microsoft.com/library/5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd%28Office.15%29.aspx) dans la réponse. Vous pouvez également rencontrer un élément enfant d’un élément [UserSettingError (SOAP)](https://msdn.microsoft.com/library/abb175c5-4f38-4dcc-81e3-b511686862eb%28Office.15%29.aspx) , s’il en existe une. Le contexte de l’erreur dépend de l’emplacement de l’élément **ErrorCode** , comme suit : 
  
- En tant qu’élément enfant de l’élément **Response** , l’élément **ErrorCode** représente une erreur qui s’applique à l’ensemble de la requête. 
    
- En tant qu’enfant de l’élément **UserResponse** , il représente une erreur qui s’applique uniquement à cet utilisateur spécifique. 
    
- En tant qu’enfant d’un élément **UserSettingError** , il représente une erreur qui s’applique à un paramètre spécifique qui a été demandé. 
    
Examinons un exemple de réponse. Dans cet exemple, l’élément **ErrorCode** sous l’élément **Response** a la valeur « NOERROR », ce qui indique une réussite globale. Toutefois, l’élément **ErrorCode** sous l’élément **UserResponse** a la valeur « RedirectAddress », ce qui indique qu’une erreur s’est produite pour cet utilisateur particulier. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
    xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>14</h:MajorVersion>
      <h:MinorVersion>3</h:MinorVersion>
      <h:MajorBuildNumber>136</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2010_SP2</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

L’article [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx) contient la liste complète des erreurs possibles. La plupart de ces éléments indiquent une erreur irrécupérable, mais quelques mérites de gestion spéciale. 
  
**Tableau 2. Valeurs de code d’découverte automatique SOAP**

|**Valeur ErrorCode**|**Pour gérer...**|
|:-----|:-----|
|RedirectAddress  <br/> |Redémarrage de la [découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l’élément [RedirectTarget (SOAP)](https://msdn.microsoft.com/library/f8162724-cf9a-4543-a1ad-5846c8b10bfa%28Office.15%29.aspx) .  <br/> |
|RedirectUrl  <br/> |[Renvoi de votre requête à une nouvelle URL](#bk_ResendRequest) vers l’URL dans l’élément **RedirectTarget** .  <br/> |
|ServerBusy  <br/> |Renouvelez cette URL après un petit délai. Vous pouvez patienter pendant un laps de temps défini ou simplement déplacer cette URL à la fin de la liste des URL à essayer. Si vous recevez cette erreur plusieurs fois à partir d’une URL, vous devez considérer que l’URL n’est pas valide.  <br/> |
   
### <a name="pox-autodiscover-errors"></a>Erreurs de découverte automatique POX

Le service de découverte automatique POX signale les erreurs un peu différemment. Les erreurs non récupérables sont contenues dans l’élément [Error (POX)](https://msdn.microsoft.com/library/91c63b62-ab68-4c32-a2f7-5a87c188335b%28Office.15%29.aspx) . L’article [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx) contient la liste complète des codes d’erreur possibles. 
  
Les erreurs de redirection sont contenues dans l’élément [action (POX)](https://msdn.microsoft.com/library/a3462c6b-453c-462a-830d-f29ee4a2babb%28Office.15%29.aspx) . Toute valeur de l’élément **action** autre que « paramètres » indique une erreur de redirection. 
  
**Tableau 3. Valeurs ErrorCode découverte automatique ErrorCode**

|**Valeur de l’action**|**Pour gérer...**|
|:-----|:-----|
|redirectAddr  <br/> |Redémarrage de la [découverte automatique avec une nouvelle adresse de messagerie](#bk_RestartAutodiscover) avec l’adresse de messagerie dans l' [RedirectAddr (POX)](https://msdn.microsoft.com/library/0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4%28Office.15%29.aspx) .  <br/> |
|redirectUrl  <br/> |[Renvoi de votre requête à une nouvelle URL](#bk_ResendRequest) vers l’URL dans l’élément [redirectUrl (POX)](https://msdn.microsoft.com/library/c54f310f-8c99-4c37-8e73-ac87722b6229%28Office.15%29.aspx) .  <br/> |
   
Dans cet exemple, l’élément **action** a la valeur « redirectAddr », ce qui indique qu’une nouvelle demande doit être envoyée avec la nouvelle adresse e-mail contenue dans l’élément **redirectAddr** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    <Account>
      <Action>redirectAddr</Action>
      <RedirectAddr>elvin@mail.contoso.com</RedirectAddr>
    </Account>
  </Response>
</Autodiscover>
```

## <a name="handling-redirect-errors"></a>Gestion des erreurs de redirection
<a name="bk_HandlingRedirects"> </a>

Vous pouvez gérer les scénarios d’erreur de redirection de deux manières :
  
- En redémarrant la découverte automatique avec une nouvelle adresse de messagerie.
    
- En renvoyant votre demande à une nouvelle URL.
    
Les deux scénarios nécessitent une validation avant de continuer.
  
### <a name="restarting-autodiscover-with-a-new-email-address"></a>Redémarrage de la découverte automatique avec une nouvelle adresse de messagerie
<a name="bk_RestartAutodiscover"> </a>

Lorsque vous obtenez une nouvelle adresse de messagerie dans une réponse de redirection de découverte automatique, vérifiez d’abord que la nouvelle adresse de messagerie fournie dans la réponse d’erreur de redirection n’est pas la même adresse que celle que vous avez envoyée dans la demande ayant provoqué l’erreur. Si c’est le cas, ne redémarrez pas la découverte automatique et considérez plutôt l’URL qui a généré la réponse pour qu’elle ne soit pas valide.
  
Si la nouvelle adresse de messagerie est différente, ignorez votre liste existante d’URL de point de terminaison de découverte automatique potentielles et générez une nouvelle liste basée sur la nouvelle adresse de messagerie.
  
### <a name="resending-your-request-to-a-new-url"></a>Renvoi de votre requête à une nouvelle URL
<a name="bk_ResendRequest"> </a>

Lorsque vous obtenez une nouvelle URL dans une réponse de redirection de découverte automatique, vous devez d’abord valider l’URL comme suit :
  
- Vérifiez que l’URL est une URL HTTPs.
    
- Vérifiez que vous n’avez pas reçu une erreur de cette URL avec l’adresse de messagerie actuelle.
    
- Si applicable à votre application, Informez l’utilisateur de la redirection et demandez-lui l’autorisation de suivre la redirection.
    
- Envoyez une demande à l’URL et [Vérifiez que le certificat SSL présenté par le serveur est valide](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).
    
Si l’URL réussit la validation, renvoyez la demande à cette nouvelle URL.
  
## <a name="see-also"></a>Voir aussi


- [Découverte automatique pour Exchange](autodiscover-for-exchange.md)
    
- [Trouver des points de terminaison de découverte automatique à l’aide de la recherche SCP dans Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [ErrorCode (SOAP)](https://msdn.microsoft.com/library/5e5ec861-0191-4ecb-a906-47ce8ed96381%28Office.15%29.aspx)
    
- [ErrorCode (POX)](https://msdn.microsoft.com/library/064d73e4-45b7-4797-828e-9df590830db8%28Office.15%29.aspx)
    

